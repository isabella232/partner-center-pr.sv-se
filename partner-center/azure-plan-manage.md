---
title: Azure-plan – Hantera prenumerationer & resurser
ms.topic: article
ms.date: 05/06/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-pricing
description: Lär dig hur partner kan använda olika alternativ för rollbaserad åtkomstkontroll (RBAC) för att få driftskontroll och hantering av en kunds Azure-resurser.
author: amitravat
ms.author: amrava
ms.localizationpriority: High
ms.custom: SEOMAY.20
ms.openlocfilehash: 14dc31f11a63520c06ee0c7c7b0a9d3830e652efd4ad75d00d7997f032af7252
ms.sourcegitcommit: 121f1b9cbd88faeba60dc9b475f9c0647cdc933c
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/06/2021
ms.locfileid: "115690364"
---
# <a name="manage-subscriptions-and-resources-under-the-azure-plan"></a>Hantera prenumerationer och resurser under Azure-planen

**Lämpliga roller:** Administratörsagent


Den här artikeln förklarar hur CSP-partner kan använda olika alternativ för rollbaserad åtkomstkontroll (RBAC) för att få driftskontroll och hantering av en kunds Azure-resurser. När du övergår en kund till Azure-planen tilldelas du privilegierade administratörsrättigheter i Azure (prenumerationens ägarrättigheter via administratör för) som standard.

 > [!NOTE]
 > Administratörsrättigheter till Azure-prenumerationen kan tas bort av kunden på prenumerations-, resursgrupps- eller arbetsbelastningsnivå. 

 Partner kan få driftkontroll och hantering av en kunds Azure-resurser i CSP dygnet runt med hjälp av olika alternativ som tillhandahålls via funktionen för rollbaserad åtkomstkontroll (RBAC). 

- **Admin on Behalf Of (AOBO)** – Med [AOBO](https://channel9.msdn.com/Series/cspdev/Module-11-Admin-On-Behalf-Of-AOBO)får alla användare med rollen Administratörsagent i partnerklientorganisationen RBAC-ägaråtkomst till Azure-prenumerationer som du skapar via CSP-programmet.

- **Azure Lighthouse:** AOBO tillåter inte flexibiliteten att skapa distinkta grupper som fungerar med olika kunder eller att aktivera olika roller för grupper eller användare. Med Azure Lighthouse kan du tilldela olika grupper till olika kunder eller roller. Eftersom användarna har rätt åtkomstnivå via Azure-delegerad resurshantering kan du minska antalet användare som har rollen administratörsagent (och därmed ha fullständig AOBO-åtkomst). Detta bidrar till att förbättra säkerheten genom att begränsa onödig åtkomst till dina kunders resurser. Det ger dig också mer flexibilitet för att hantera flera kunder i stor skala. Mer information finns i [Azure Lighthouse och Molnlösningsleverantör program](/azure/lighthouse/concepts/cloud-solution-provider).

- **Katalog- eller [](/azure/active-directory/develop/app-objects-and-service-principals)gästanvändare** eller tjänsthuvudnamn: Du kan delegera detaljerad åtkomst till CSP-prenumerationer genom att lägga till användare i kundkatalogen eller lägga till gästanvändare och tilldela specifika RBAC-roller.

Microsoft rekommenderar att användarna har den lägsta behörighet de behöver för att utföra sitt arbete som en säkerhetspraxis. Se [Azure Active Directory Privileged Identity Management resurser](/azure/active-directory/privileged-identity-management/pim-configure).

## <a name="link-your-partner-id-mpn-id-to-your-credentials-for-managing-customers-azure-resources"></a>Länka ditt partner-ID (MPN-ID) till dina autentiseringsuppgifter för att hantera kundens Azure-resurser

I följande tabell visas de metoder som används för att associera ditt partner-ID med olika RBAC-åtkomstalternativ.

|**Kategori**   |**Scenario**   |**MPN ID-association**|
|-----------------|:------------------------|:------------------|
|Aobo   |CSP direkt partner eller indirekt leverantör skapar prenumerationen för kunden som gör CSP direkt partner eller indirekt provider standardägare för prenumerationen med hjälp av AOBO. CSP-direkt partner eller indirekt leverantör ger indirekt återförsäljare åtkomst till prenumerationen med hjälp av AOBO.|Automatiskt (inget partnerarbete krävs)|
|Azure Lighthouse|Partner skapar ett nytt [erbjudande för hanterade tjänster på Marketplace.](/azure/lighthouse/concepts/managed-services-offers) Det här erbjudandet accepteras i CSP-prenumerationen och partnern får åtkomst till CSP-prenumerationen.|Automatiskt (inget partnerarbete krävs)|
|Azure Lighthouse|Partner distribuerar [ARM-mall i](/azure/lighthouse/how-to/onboard-customer) En Azure-prenumeration|Partnern måste associera MPN-ID:t med användaren eller tjänstens huvudnamn i partnerklientorganisationen. Mer information finns i [Länka Partner-ID](/azure/billing/billing-partner-admin-link-started).|
|Katalog- eller gästanvändare|Partnern skapar en ny användare eller tjänstens huvudnamn i kundkatalogen och ger användaren åtkomst till CSP-prenumerationen. Partner skapar en ny användare eller tjänstens huvudnamn i kundkatalogen. Partner lägger till användaren i en grupp och ger åtkomst till CSP-prenumerationen till gruppen.|Partnern måste associera MPN-ID:t med användaren eller tjänstens huvudnamn i kundens klientorganisation. Mer information finns i [Länka Partner-ID](/azure/billing/billing-partner-admin-link-started).|

## <a name="confirm-that-you-have-admin-access"></a>Bekräfta att du har administratörsåtkomst

Du behöver administratörsåtkomst för att hantera kundens tjänster och för att få intjänade krediter. Läs [Partner-intjänade krediter](partner-earned-credit.md) för detaljerad information om intjänade krediter. Du kan kontrollera att du har administratörsåtkomst på två sätt.

- Granska filen för daglig användning – Detta kan fastställas genom att granska enhetspriset och det effektiva enhetspriset i filen för daglig användning och bekräfta om en rabatt tillämpas. Om du får rabatten är du administratör.

- Skapa en Azure Monitor-avisering – Du kan [](/azure/azure-monitor/platform/alerts-activity-log) skapa en Azure Monitor aktivitetsloggavisering som ska meddelas om när din RBAC-åtkomst tas bort från CSP-prenumerationen.

### <a name="create-an-azure-monitor-alert"></a>Skapa en Azure Monitor-avisering

1. Skapa avisering.

   :::image type="content" source="images/azure/azurealert1.png" alt-text="azure-avisering.":::

2. Välj den typ av åtgärd som du vill att aviseringen ska vidta. Om du till exempel anger att du vill ha ett e-postmeddelande får du ett e-postmeddelande med ett meddelande om borttagning av rolltilldelningar.

   :::image type="content" source="images/azure/azureconfigurealert2.png" alt-text="konfigurera avisering.":::

### <a name="aobo-removal"></a>Borttagning av AOBO

Kunder kan hantera åtkomst till sina prenumerationer genom att **gå Access Control** på Azure Portal. På fliken **Rolltilldelningar** väljer de Ta **bort åtkomst.** Om detta inträffar kan du:

- Prata med kunden för att se om administratörsåtkomst kan återställas.

- Använd den åtkomst som tillhandahålls [via rollbaserad åtkomstkontroll (RBAC).](/azure/role-based-access-control/overview)

- Använd åtkomst som tillhandahålls via [Azure Lighthouse](https://azure.microsoft.com/services/azure-lighthouse/).

Rollbaserad åtkomst skiljer sig från administratörsåtkomst. Roller avgränsar exakt vad du kan och inte kan göra. Administratörsåtkomst är bredare.

Om du vill se vilka roller som är berättigade till PEC läser du [Roller och behörigheter för partnerns intjänade kredit](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RE3QuW2).

## <a name="next-steps"></a>Nästa steg

- [Återkalla och omvärderar administratörsbehörigheter för Azure CSP prenumerationer](revoke-reinstate-csp.md)

- [Partner-intjänad kredit – översikt](partner-earned-credit.md)

- [Partner-intjänad kredit för hanterade tjänster](partner-earned-credit-explanation.md)