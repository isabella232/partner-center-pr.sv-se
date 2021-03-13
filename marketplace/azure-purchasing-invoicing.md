---
title: Köpa program vara och lösningar från Azure Marketplace
description: Lär dig mer om verktyg som fören klar och effektiviserar program varu inköp och-hantering i Azure Marketplace.
ms.service: marketplace-customer
ms.topic: conceptual
author: Guyshu
ms.author: gushuchm
ms.date: 01/18/2021
ms.openlocfilehash: ac20b3c0603f886104499ab8de6da1d3459bbd57
ms.sourcegitcommit: 3a2415ab9833d5c574ad76d462f526a131c24f33
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/12/2021
ms.locfileid: "103412581"
---
# <a name="azure-marketplace-purchasing"></a>Köp av Azure Marketplace

Azure Marketplace har flera verktyg och funktioner som fören klar och fören klar processen att köpa, fakturera och hantera inköps principer.

## <a name="simplified-procurement"></a>Förenklad upphandling

Azure Marketplace förenklar anskaffningsprocessen via olika inköpsalternativ. Om du köper produkter med hjälp av ett kredit kort som är kopplat till ditt Azure-konto kommer alla inköp att samlas på en enda faktura och faktureras enligt det kredit kort som du väljer. Om du är en stor kund kan du köpa med en Enterprise-avtal. Med ett EA, inkluderas alla program varu inköp automatiskt i din Azure-faktura. Din faktura kommer att innehålla Azure-användningsavgifter först, följt av Azure Marketplace-avgifter.

När du köper via Azure Marketplace eliminerar du komplexiteten med att hantera enskilda leverantörs relationer och fakturor. Du får en enkel, sammanställd månatlig faktura från Microsoft som omfattar både dina Azure Marketplace-köp och dina Azure-kostnader.

## <a name="permission-to-purchase"></a>Behörighet att köpa

När du har hittat rätt program vara är det enkelt att slutföra köpet. Du kommer dock att behöva lämpliga behörigheter i Azure-prenumerationen. Eftersom Azure fungerar på en [rollbaserad Access Control](/azure/role-based-access-control/overview) (RBAC)-modell måste ditt konto ha **prenumerations ägarens** eller **deltagar** behörighet för att göra ett köp.

Innan du slutför ett köp måste du se till att användaren har rätt konfiguration i Azure-klienten. Detta bidrar till att förhindra fel under köpet.

I Azure Marketplace-upplevelsen i Azure Portal letar du reda på det program som du vill köpa och väljer **skapa** eller **Konfigurera + prenumerera**. Du uppmanas att slutföra viss information innan du kan använda den nya lösningen.

:::image type="content" source="media/overview/offer-create-screen.png" alt-text="Knappen Skapa erbjudande.":::

:::image type="content" source="media/overview/button-set-up-and-subscribe.png" alt-text="Knappen Konfigurera + prenumerera.":::

Om du vill distribuera en lösning från Azure Marketplace Online Store väljer du **Hämta nu** på sidan produkt beskrivning och loggar sedan in med dina autentiseringsuppgifter för Azure-kontot.

:::image type="content" source="media/overview/sign-in-to-azure-marketplace.png" alt-text="Dialog rutan inloggning i Azure Marketplace.":::

När du har loggat in kommer du att omdirigeras till produkten i Azure Portal för att slutföra köpet.

## <a name="purchase-policy-management"></a>Hantering av inköps princip

Med Microsoft kan du hantera användar inköp via din fakturerings profil som administratör för Azure-prenumerationen. Välj mellan tre alternativ:

- **Kostnads fri + betald** – ger användare möjlighet att köpa valfritt program för Azure Marketplace.
- **Kostnads fri** – tillåter att användare bara distribuerar gratis program vara från Azure Marketplace.
- **Nej** – hindrar användare från att distribuera program vara från Azure Marketplace.

De här inställningarna gäller för alla användare som har åtkomst till din Azure-prenumeration, vilket ger dig möjlighet att styra IT-förhandlingen genom Azure Portal.

:::image type="content" source="media/overview/billing-profile-policy-settings.png" alt-text="Styra IT-tillvaratagande via Azure Portal":::

## <a name="cost-management"></a>Kostnadshantering

När du köper produkter från Azure Marketplace vill du få insikter som hjälper dig att hantera kostnader. Azure Cost Management är ett kostnads fritt verktyg för att visa information om de produkter som du har köpt. Du kan använda Cost Management för att se information om vilka tjänster du kostar pengar på, och hur dessa kostnader går igenom de budgetar som du har angett. Förutom att ställa in budgetar kan du schemalägga rapporter och analysera prenumerations kostnader. Läs mer om Azure Cost Management genom att fylla i modulen Microsoft Learn på [Analysera kostnader och skapa budgetar med Azure Cost Management](/learn/modules/analyze-costs-create-budgets-azure-cost-management/).

Du kan visa dina Azure Marketplace-avgifter och fakturor i kostnadsanalysverktyget under Azure Cost Management.

:::image type="content" source="media/overview/azure-cost-management.png" alt-text="Använd Azure Cost Management för att få insikter om dina köpta produkter.":::

## <a name="purchase-validation-checks"></a>Verifierings kontroller för inköp

Att köpa ett erbjudande via Azure Marketplace kan inte utföras av olika orsaker. Att använda kommando rads gränssnittet (CLI) för ett köp är mer sannolikt att orsaka fel eftersom du kanske försöker köpa ett erbjudande som inte är tillgängligt eller synligt i Azure Marketplace. Nedan visas de kontroller som kan göra att ett köp inte kan utföras:

1. Prenumerationen tillhör ett Enterprise-avtal (EA) och EA-administratören inaktiverade Azure Marketplace-köp.
1. Funktionen EA admin har endast aktiverat inköp för kostnads fria erbjudanden och erbjudandet är ett betalt erbjudande.
1. Erbjudandet finns inte på Marketplace.
1. Oberoende program varu leverantörer (ISV) slutade sälja erbjudandet, minst i din region.
1. Den prenumeration som du använder tillhör ett fakturerings konto i en region där erbjudandet inte är tillgängligt.
1. Prenumerations-/fakturerings kontot är inte associerat med en giltig betalnings metod (till exempel ett giltigt kredit kort).
1. Prenumerationen tillhör en leverantör av moln lösningar (CSP) och ISV nekade att sälja via en KRYPTOGRAFIPROVIDER.
1. En privat Marketplace har Aktiver ATS för prenumerationen och erbjudandet finns inte i listan över tillåtna erbjudanden.
1. Erbjudandet är privat/för hands version för vissa kunder och prenumerationen finns inte i listan över tillåtna kunder.

## <a name="next-steps"></a>Nästa steg

- [Fakturering](billing-invoicing.md)