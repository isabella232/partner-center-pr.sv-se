---
title: Azure-plan – hantera prenumerationer & resurser
ms.topic: article
ms.date: 05/06/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Lär dig hur partner kan använda olika RBAC-alternativ (rollbaserad åtkomst kontroll) för att få drift kontroll och hantering av en kunds Azure-resurser.
author: amitravat
ms.author: amrava
ms.localizationpriority: High
ms.custom: SEOMAY.20
ms.openlocfilehash: 31e9c6862a5aa19407fa6da5e15333bb7e696720
ms.sourcegitcommit: 2d9aab15ddc20cb3d9537e68ace33d36f7d8a250
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 12/02/2020
ms.locfileid: "96534938"
---
# <a name="manage-subscriptions-and-resources-under-the-azure-plan"></a>Hantera prenumerationer och resurser under Azure-planen

**Lämpliga roller**

- Administratörs agent


Den här artikeln förklarar hur CSP-partner kan använda olika alternativ för rollbaserad åtkomst kontroll (RBAC) för att få drift kontroll och hantering av en kunds Azure-resurser. När du övergår till en kund i Azure-planen tilldelas du som standard privilegierade administratörs rättigheter i Azure (prenumerations ägarens rättigheter via admin).

 > [!NOTE]
 > Administratörs behörighet till Azure-prenumerationen kan tas bort av kunden på en prenumeration, resurs grupp eller arbets belastnings nivå. 

 Partner kan få dygnet runt drift styrning och hantering av en kunds Azure-resurser i CSP genom att använda olika alternativ som tillhandahålls via den rollbaserade funktionen för åtkomst kontroll (RBAC). 

- **Administratör på uppdrag av (administrate)** – med [administrate](https://channel9.msdn.com/Series/cspdev/Module-11-Admin-On-Behalf-Of-AOBO), kommer alla användare med rollen admin agent i partner klienten att ha RBAC-ägare till gång till Azure-prenumerationer som du skapar via CSP-programmet.

- **Azure Lighthouse**: administrate tillåter inte flexibiliteten att skapa distinkta grupper som fungerar med olika kunder, eller för att aktivera olika roller för grupper eller användare. Med Azure Lighthouse kan du tilldela olika grupper till olika kunder eller roller. Eftersom användarna får rätt åtkomst nivå via Azure-delegerad resurs hantering kan du minska antalet användare som har rollen administratörs agent (och därmed ha fullständig ADMINISTRATE-åtkomst). Detta bidrar till att förbättra säkerheten genom att begränsa onödig åtkomst till dina kunders resurser. Det ger dig också större flexibilitet att hantera flera kunder i stor skala. Mer information finns i [Azure-Lighthouse och Cloud Solution Provider-programmet](/azure/lighthouse/concepts/cloud-solution-provider).

- **Katalog-eller gäst användare eller [tjänst huvud namn](/azure/active-directory/develop/app-objects-and-service-principals)**: du kan delegera detaljerad åtkomst till CSP-prenumerationer genom att lägga till användare i kund katalogen eller lägga till gäst användare och tilldela specifika RBAC-roller.

Microsoft rekommenderar att användarna har de lägsta behörigheter som de behöver för att utföra sitt arbete som säkerhets praxis. Se [Azure Active Directory Privileged Identity Management-resurser](/azure/active-directory/privileged-identity-management/pim-configure).

## <a name="link-your-partner-id-mpn-idto-your-credentials-for-managing-customers-azure-resources"></a>Länka ditt partner-ID (MPN-ID) till dina autentiseringsuppgifter för att hantera kundens Azure-resurser

I följande tabell visas de metoder som används för att associera ditt partner-ID med olika RBAC-åtkomst alternativ.

|**Kategori**   |**Scenario**   |**Association för MPN-ID**|
|-----------------|:------------------------|:------------------|
|ADMINISTRATE   |CSP Direct-partner eller en indirekt Provider skapar prenumerationen för kunden som gör CSP Direct-partnern eller den indirekta providerns standard ägare av prenumerationen med hjälp av ADMINISTRATE. CSP Direct-partner eller indirekt Provider ger indirekt åter försäljare åtkomst till prenumerationen med hjälp av ADMINISTRATE.|Automatiskt (ingen partner arbete krävs)|
|Azure Lighthouse|Partner skapar ett nytt [erbjudande för hanterade tjänster i Marketplace](/azure/lighthouse/concepts/managed-services-offers). Erbjudandet accepteras av CSP-prenumerationen och partnern får åtkomst till CSP-prenumerationen.|Automatiskt (ingen partner arbete krävs)|
|Azure Lighthouse|Partner distribuerar [arm-mallen](/azure/lighthouse/how-to/onboard-customer) i Azure-prenumerationen|Partner måste associera MPN-ID: t till användarens eller tjänstens huvud namn i partner klient organisationen. Mer information – [länk partner-ID](/azure/billing/billing-partner-admin-link-started).|
|Katalog eller gäst användare|Partner skapar en ny användare eller tjänstens huvud namn i kund katalogen och ger åtkomst till CSP-prenumerationen för användaren. Partner skapar en ny användare eller tjänstens huvud namn i kund katalogen. Partner lägger till användaren i en grupp och ger åtkomst till CSP-prenumerationen till gruppen.|Partner måste associera MPN-ID: t till användarens eller tjänstens huvud namn i kund klienten. Mer information – [länk partner-ID](/azure/billing/billing-partner-admin-link-started).|

## <a name="confirm-that-you-have-admin-access"></a>Bekräfta att du har administratörs åtkomst

Du behöver administratörs behörighet för att hantera kundens tjänster och ta emot intjänade krediter. Läs de [intjänade krediterna för partner](partner-earned-credit.md) för detaljerad information om intjänade krediter. Du kan se till att du har administratörs behörighet på två sätt.

- Granska den dagliga användnings filen – detta kan fastställas genom att granska enhets priset och det effektiva enhets priset i den dagliga användnings filen och bekräfta om en rabatt tillämpas. Om du får rabatten som du är administratör.

- Skapa en avisering om Azure Monitor – du kan skapa en Azure Monitor aktivitets logg [avisering](/azure/azure-monitor/platform/alerts-activity-log) som meddelas när din RBAC-åtkomst tas bort från CSP-prenumerationen.

### <a name="create-an-azure-monitor-alert"></a>Skapa en Azure Monitor-avisering

1. Skapa avisering.

   :::image type="content" source="images/azure/azurealert1.png" alt-text="Azure-avisering":::

2. Välj den typ av åtgärd som du vill att aviseringen ska utföra. Om du till exempel anger att du vill ha ett e-postmeddelande får du ett meddelande om att borttagning av roll tilldelningar sker.

   :::image type="content" source="images/azure/azureconfigurealert2.png" alt-text="Konfigurera avisering":::

### <a name="aobo-removal"></a>Borttagning av ADMINISTRATE

Kunder kan hantera åtkomsten till sina prenumerationer genom att gå till **Access Control** på Azure Portal. På fliken **roll tilldelningar** väljer du **ta bort åtkomst**. I så fall kan du:

- Prata med kunden för att se om administratörs åtkomst kan återställas.

- Använd åtkomst som tillhandahålls via [rollbaserad åtkomst kontroll (RBAC)](/azure/role-based-access-control/overview).

- Använd åtkomst som tillhandahålls via [Azure Lighthouse](https://azure.microsoft.com/services/azure-lighthouse/).

Rollbaserad åtkomst skiljer sig från administratörs åtkomst. Roller begränsar exakt vad du kan och inte kan göra. Administratörs åtkomsten är bredare.

Om du vill se vilka roller som har behörighet att tjäna PEC, Läs [roller och behörigheter för den intjänade partner krediten](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RE3QuW2).

## <a name="next-steps"></a>Nästa steg

- [Återkalla och återinför administratörs behörighet för Azure CSP-prenumerationer](revoke-reinstate-csp.md)

- [Partner intjänad kredit – översikt](partner-earned-credit.md)

- [Partner intjänad kredit för hanterade tjänster](partner-earned-credit-explanation.md)