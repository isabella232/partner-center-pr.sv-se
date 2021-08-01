---
title: Köpa programvara och lösningar från Azure Marketplace
description: Lär dig mer om verktyg som förenklar och effektiviserar programvaruinköp och -hantering i Azure Marketplace.
ms.service: marketplace-customer
ms.topic: conceptual
author: Guyshu
ms.author: gushuchm
ms.date: 06/22/2021
ms.openlocfilehash: 42e08be73fb6bd1b26e75f461ede51b1e18b909b
ms.sourcegitcommit: b53616cd7bfeb68298dee69935a8007827b19d21
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/01/2021
ms.locfileid: "115014708"
---
# <a name="azure-marketplace-purchasing"></a>Azure Marketplace köp

Azure Marketplace har flera verktyg och funktioner som förenklar och effektiviserar inköpsprocessen, faktureringen och hanteringen av inköpsprincipen.

## <a name="simplified-procurement"></a>Förenklad anskaffning

Azure Marketplace förenklar anskaffningsprocessen via olika inköpsalternativ. Om du köper produkter med ett kreditkort som är associerat med ditt Azure-konto konsolideras alla inköp på en enda faktura och faktureras till det kreditkort du väljer. Om du är en stor kund kan du köpa med hjälp av en företagsavtal. Med ett EA inkluderas alla programvaruinköp automatiskt på din Azure-faktura. Din faktura kommer att innehålla Azure-användningsavgifter först, följt av Azure Marketplace-avgifter.

När du köper via Azure Marketplace eliminerar du komplexiteten med att hantera enskilda leverantörsrelationer och fakturor. Du får en enda konsoliderad månadsfaktura från Microsoft som innehåller både dina Azure Marketplace-inköp och dina Azure-avgifter.

## <a name="permission-to-purchase"></a>Behörighet att köpa

När du har hittat rätt program är det enkelt att slutföra köpet. Du behöver dock lämpliga behörigheter i Azure-prenumerationen. Eftersom Azure använder en RBAC-modell [(rollbaserad Access Control)](/azure/role-based-access-control/overview) måste  ditt  konto ha ägar- eller deltagarbehörighet för prenumerationen för att kunna göra ett köp.

Innan du slutför ett köp kontrollerar du att användaren har rätt konfiguration i Azure-klientorganisationen. Detta hjälper till att förhindra fel under köpet.

I den Azure Marketplace upplevelsen i Azure Portal du det program som du vill köpa och väljer **Skapa** **eller Konfigurera + prenumerera.** Du uppmanas att slutföra en del information innan du kan använda den nya lösningen.

> [!CAUTION]
> Godkännande till privat Marketplace anger inte anskaffning av en lösning.

:::image type="content" source="media/overview/offer-create-screen.png" alt-text="Knappen Skapa för erbjudandet.":::

:::image type="content" source="media/overview/button-set-up-and-subscribe.png" alt-text="Knappen Konfigurera + prenumerera.":::

Om du vill distribuera en lösning från Azure Marketplace onlinebutik väljer du Hämta **nu** på produktbeskrivningssidan och loggar sedan in med dina autentiseringsuppgifter för Azure-kontot.

:::image type="content" source="media/overview/sign-in-to-azure-marketplace.png" alt-text="Dialogrutan Azure Marketplace inloggning.":::

När du har loggat in omdirigeras du till produkten i Azure Portal slutföra köpet.

## <a name="purchase-policy-management"></a>Hantering av köpprincip

Med Microsoft kan du hantera användarinköp via din faktureringsprofil som Azure-prenumerationsadministratör. Välj mellan tre alternativ:

- **Kostnadsfri + betald** – Tillåter användare att skaffa alla Azure Marketplace-program.
- **Kostnadsfri** – Tillåter användare att endast distribuera kostnadsfri programvara från Azure Marketplace.
- **Nej** – Förhindrar att användare distribuerar programvara från Azure Marketplace.

De här inställningarna gäller för alla användare med åtkomst till din Azure-prenumeration, vilket ger dig möjlighet att kontrollera IT-anskaffning via Azure Portal.

:::image type="content" source="media/overview/billing-profile-policy-settings.png" alt-text="Kontrollera IT-anskaffning via Azure Portal.":::

## <a name="cost-management"></a>Kostnadshantering

När du köper produkter från Azure Marketplace vill du få insikter som hjälper dig att hantera kostnader. Azure Cost Management är ett kostnadsfritt verktyg för att visa information om de produkter som du har köpt. Du kan använda Cost Management för att se information om vilka tjänster du spenderar pengar på över tid och hur dessa kostnader spåras mot de budgetar som du har angett. Förutom att ange budgetar kan du schemalägga rapporter och analysera prenumerationskostnader. Läs mer om Azure Cost Management genom att slutföra modulen Microsoft Learn Analysera kostnader och [skapa budgetar med Azure Cost Management](/learn/modules/analyze-costs-create-budgets-azure-cost-management/).

Du kan visa dina Azure Marketplace-avgifter och fakturor i kostnadsanalysverktyget under Azure Cost Management.

:::image type="content" source="media/overview/azure-cost-management.png" alt-text="Använd Azure Cost Management för att få insikter om dina köpta produkter.":::

## <a name="purchase-validation-checks"></a>Valideringskontroller för köp

Att köpa ett erbjudande via Azure Marketplace kan misslyckas av olika orsaker. Att använda kommandoradsgränssnittet (CLI) för ett köp är mer troligt att orsaka fel eftersom du kanske försöker köpa ett erbjudande som inte är tillgängligt eller synligt i Azure Marketplace. Följande är de kontroller som kan orsaka att ett köp misslyckas:

1. Prenumerationen tillhör en företagsavtal (EA) och EA-administratören inaktiverade Azure Marketplace inköp.
1. EA-administratören har endast aktiverat köp för kostnadsfria erbjudanden och erbjudandet är ett betalt erbjudande.
1. Erbjudandet finns inte på Marketplace.
1. Oberoende programvaruleverantör (ISV) slutade sälja erbjudandet, åtminstone i din region.
1. Prenumerationen som du använder tillhör ett faktureringskonto i en region där erbjudandet inte är tillgängligt.
1. Prenumerationen/faktureringskontot är inte associerat med ett giltigt betalningsmedel (till exempel ett giltigt kreditkort).
1. Prenumerationen tillhör en Molnlösningsleverantör (CSP) och ISV:n avböjde att sälja via en CSP.
1. Privat Marketplace har aktiverats för prenumerationen och erbjudandet finns inte med i listan över tillåtna erbjudanden.
1. Erbjudandet är privat/förhandsversion för specifika kunder och prenumerationen finns inte med i listan över tillåtna kunder.

> [!NOTE]
> Köp av Marketplace-erbjudanden kan misslyckas om det står i konflikt Azure Policy som definierats av Azure-administratören i din organisation. Du kan till exempel inte köpa Microsoft.SaaS om det inte finns i organisationens **lista över tillåtna.** Mer information finns i [Azure Policy dokumentation.](/azure/governance/policy/)

## <a name="next-steps"></a>Nästa steg

- [Fakturering](billing-invoicing.md)