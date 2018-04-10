---
title: "Zuordnen von Artikelzu-/-abschlägen zu Einkäufen oder Verkäufen| Microsoft Docs"
description: "Wenn Sie Ihren Lagerartikel Kosten wie Fracht, Versicherung, Umlagerung und Transport hinzufügen möchten, die beim Kauf oder Verkauf entstehen, können Sie die Artikelgebührenfunktion verwenden."
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: transportation, added cost
ms.date: 06/06/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: d7fb34e1c9428a64c71ff47be8bcff174649c00d
ms.openlocfilehash: 717090789c380bee19f12882fc4fc6ade76c8420
ms.contentlocale: de-de
ms.lasthandoff: 03/22/2018

---
# <a name="use-item-charges-to-account-for-additional-trade-costs"></a><span data-ttu-id="7acb6-103">Verwenden von Artikelzuschlägen für zusätzliche Kosten</span><span class="sxs-lookup"><span data-stu-id="7acb6-103">Use Item Charges to Account for Additional Trade Costs</span></span>
<span data-ttu-id="7acb6-104">Um eine korrekte Bewertung sicherzustellen, müssen Ihre Lagerartikel Kosten wie Fracht, Versicherung, Umlagerung und Transport enthalten, die beim Kauf oder Verkauf entstehen.</span><span class="sxs-lookup"><span data-stu-id="7acb6-104">To ensure correct valuation, your inventory items must carry any added costs, such as freight, physical handling, insurance, and transportation that you incur when purchasing or selling the items.</span></span> <span data-ttu-id="7acb6-105">Die Kosten eines eingekauften Artikels bestehen aus dem Einkaufspreis des Kreditors und allen zusätzlichen Artikelzuschlägen, die einzelnen Wareneingängen oder Rücklieferungen zugewiesen werden können.</span><span class="sxs-lookup"><span data-stu-id="7acb6-105">For purchases, the landed cost of a purchased item consists of the vendor's purchase price and all additional direct item charges that can be assigned to individual receipts or return shipments.</span></span> <span data-ttu-id="7acb6-106">Die Frachtkosten der verkauften Artikel zu kennen, kann für Ihr Unternehmen genauso wichtig sein wie die Einkaufspreise der eingekauften Artikel zu kennen.</span><span class="sxs-lookup"><span data-stu-id="7acb6-106">For sales, knowing the cost of shipping sold items can be as vital to your company as knowing the landed cost of purchased items.</span></span>

<span data-ttu-id="7acb6-107">Zusätzlich zum Aufzeichnen der hinzugefügten Kosten zum Lagerwert, können Sie die Funktion Artikelzuschlag wie folgt verwenden:</span><span class="sxs-lookup"><span data-stu-id="7acb6-107">In addition to recording the added cost in you inventory value, you can use the Item Charges feature for the following:</span></span>

- <span data-ttu-id="7acb6-108">Die Identifizierung der Gesamtkosten eines Artikels, um bessere Entscheidungen bezüglich der Optimierung des Vertriebsnetzes zu treffen.</span><span class="sxs-lookup"><span data-stu-id="7acb6-108">Identify the landed cost of an item for making more accurate decisions on how to optimize the distribution network.</span></span>
- <span data-ttu-id="7acb6-109">Die Analyse der Zusammensetzung eines Verkaufspreises/Einstandspreises eines Artikels.</span><span class="sxs-lookup"><span data-stu-id="7acb6-109">Break down the unit cost or unit price of an item for analysis purposes.</span></span>
- <span data-ttu-id="7acb6-110">Die Einberechnung von Einkaufsrabatten in den Einstandspreis und von Verkaufsrabatten in den Verkaufspreis.</span><span class="sxs-lookup"><span data-stu-id="7acb6-110">include purchase allowances into the unit cost and sales allowances into the unit price.</span></span>

<span data-ttu-id="7acb6-111">Bevor Sie Artikeln Gebühren zuweisen können, müssen Sie Artikelchargennummern für unterschiedliche Artikelarten zuweisen, inklusive Sachkontokosten, die mit Verkäufen, Einkäufen und Lagerregulierungen verknüpft sind.</span><span class="sxs-lookup"><span data-stu-id="7acb6-111">Before you can assign item charges, you must set up item charge numbers for the different types of item charges, including to which G/L accounts costs related to sales, purchases, and inventory adjustments are posted to.</span></span> <span data-ttu-id="7acb6-112">Eine Artikelzuschlagsnummer enthält eine Kombination von Produktbuchungsgruppe, Steuergruppencode, MwSt.-Produktbuchungsgruppe und Artikelzuschlag.</span><span class="sxs-lookup"><span data-stu-id="7acb6-112">An item charge number contains a combination of general product posting group, tax group code, VAT product posting group, and item charge.</span></span> <span data-ttu-id="7acb6-113">Wenn Sie die Nummer des Artikel Zu-/Abschlags in einen Einkaufs- oder Verkaufsbeleg eingeben, ermittelt die Anwendung ein Sachkonto auf der Basis der Einrichtung des Artikel Zu-/Abschlags und der Informationen im jeweiligen Beleg.</span><span class="sxs-lookup"><span data-stu-id="7acb6-113">When you enter the item charge number on a purchase or sales document, the relevant G/L account is retrieved based on the setup of the item charge number and the information on the document.</span></span>

<span data-ttu-id="7acb6-114">Für Bestellungen und Verkaufsbelege können Artikelzuschläge auf zwei Arten zugeordnet werden:</span><span class="sxs-lookup"><span data-stu-id="7acb6-114">For both purchase and sales documents, you can assign an item charge in two ways:</span></span>
- <span data-ttu-id="7acb6-115">Auf dem Beleg, auf dem der Artikel aufgeführt ist, auf den sich der Artikelzuschlag bezieht.</span><span class="sxs-lookup"><span data-stu-id="7acb6-115">On the document where the items that the item charge relates to are listed.</span></span> <span data-ttu-id="7acb6-116">Dies ist in der Regel für Belege der Fall, die noch nicht vollständig gebucht sind.</span><span class="sxs-lookup"><span data-stu-id="7acb6-116">This you typically do for documents that are not yet fully posted.</span></span>
- <span data-ttu-id="7acb6-117">Auf einer getrennten Rechnung, indem Sie den Artikelzuschhlag mit einem gebuchten Beleg oder einer Lieferung verknüpfen, in denen der Artikel vorkommt, zu dem der Artikelzuschlag gehört.</span><span class="sxs-lookup"><span data-stu-id="7acb6-117">On a separate invoice by linking the item charge to a posted receipt or shipment where the items that the item charge relate to are listed.</span></span>

> [!NOTE]  
>   <span data-ttu-id="7acb6-118">Sie können Artikelzuschläge in Bestellungen, Rechnungen und Gutschriften für Verkaufs- und Einkaufsberichte zuweisen.</span><span class="sxs-lookup"><span data-stu-id="7acb6-118">You can assign item charges to orders, invoices, and credit memos, for both sales and purchases.</span></span> <span data-ttu-id="7acb6-119">Die folgenden Verfahren beschreiben, wie man mit Artikelzuschlägen für eine Einkaufsrechnung arbeitet.</span><span class="sxs-lookup"><span data-stu-id="7acb6-119">The following procedures describe how to work with item charges for a purchase invoice.</span></span> <span data-ttu-id="7acb6-120">Die Schritte sind für alle anderen Einkaufs- und Verkaufsbelege ähnlich.</span><span class="sxs-lookup"><span data-stu-id="7acb6-120">The steps are similar for all other purchase and sales documents.</span></span>

## <a name="to-set-up-item-charge-numbers"></a><span data-ttu-id="7acb6-121">Vorgehensweise: Eine Artikelzu-/-abschlagsnummer einrichten</span><span class="sxs-lookup"><span data-stu-id="7acb6-121">To set up item charge numbers</span></span>
<span data-ttu-id="7acb6-122">Sie können die Artikel Zu-/Abschlagsnummern verwenden, um die verschiedenen Arten von Artikel Zu-/Abschlägen, die in Ihrem Unternehmen verwendet werden, zu verwalten.</span><span class="sxs-lookup"><span data-stu-id="7acb6-122">You use item charge numbers to distinguish between the different kinds of item charges that are used in your company.</span></span>

1. <span data-ttu-id="7acb6-123">Wählen Sie in der rechten oberen Ecke das Symbol ![Nach Seite oder Bericht suchen](media/ui-search/search_small.png "Nach Seite oder Bericht suchen") und geben **Artikel-Gebühren** ein und wählen den zugehörenden Link aus.</span><span class="sxs-lookup"><span data-stu-id="7acb6-123">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Item Charges**, and then choose the related link.</span></span>
2. <span data-ttu-id="7acb6-124">Wählen Sie im Fenster **Artikel-Gebühren** die Aktion **Neu** aus, um eine neue Zeile für eine zu erstellen.</span><span class="sxs-lookup"><span data-stu-id="7acb6-124">In the **Item Charges** window, choose the **New** action to create a new line.</span></span>
3. <span data-ttu-id="7acb6-125">Füllen Sie die Felder je nach Bedarf aus.</span><span class="sxs-lookup"><span data-stu-id="7acb6-125">Fill in the fields as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]

## <a name="to-assign-an-item-charge-directly-to-the-purchase-invoice-for-the-item"></a><span data-ttu-id="7acb6-126">Um einen Artikel Zu-/Abschlag in die Einkaufsrechnung für den Artikel zuordnen</span><span class="sxs-lookup"><span data-stu-id="7acb6-126">To assign an item charge directly to the purchase invoice for the item</span></span>
<span data-ttu-id="7acb6-127">Wenn Sie den Artikel-Zu-/Abschlag kennen, und den Zeitpunkt Sie eine Einkaufsrechnung für den Artikel betreffen, gehen Sie folgendermaßen vor.</span><span class="sxs-lookup"><span data-stu-id="7acb6-127">If you know the item charge at the time when you post a purchase invoice for the item, follow this procedure.</span></span>

1. <span data-ttu-id="7acb6-128">Wählen Sie das Symbol ![Nach Seite oder Bericht suchen](media/ui-search/search_small.png "Nach Seite oder Bericht suchen") und geben **Gebuchte Einkaufsrechnungen** ein. Wählen Sie dann den zugehörigen Link aus.</span><span class="sxs-lookup"><span data-stu-id="7acb6-128">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Purchase Invoices**, and then choose the related link.</span></span>
2. <span data-ttu-id="7acb6-129">Eine neue Einkaufsrechnung erstellen.</span><span class="sxs-lookup"><span data-stu-id="7acb6-129">Create a new purchase invoice.</span></span> <span data-ttu-id="7acb6-130">Weitere Informationen finden Sie unter [Erfassen eines Einkaufs](purchasing-how-record-purchases.md).</span><span class="sxs-lookup"><span data-stu-id="7acb6-130">For more information, see [Record Purchases](purchasing-how-record-purchases.md).</span></span>
3. <span data-ttu-id="7acb6-131">Stellen Sie sicher, dass die Einkaufsrechnung eine oder mehrere Zeilen vom Artikeltyp hat.</span><span class="sxs-lookup"><span data-stu-id="7acb6-131">Make sure the purchase invoice has one or more lines of type Item.</span></span>
4. <span data-ttu-id="7acb6-132">Geben Sie eine neue Zeile ein, und wählen Sie **Zu-/Abschlag (Artikel)** im Feld **Art**.</span><span class="sxs-lookup"><span data-stu-id="7acb6-132">On a new line, in the **Type** field, select **Charge (Item)**.</span></span>
5. <span data-ttu-id="7acb6-133">Geben Sie in dem Feld **Menge** die Anzahl der Einheiten dieses Artikel Zu-/Abschlages ein, für die Sie eine Rechnung erhalten haben.</span><span class="sxs-lookup"><span data-stu-id="7acb6-133">In the **Quantity** field, enter the units of the item charge that you have been invoiced for.</span></span>
6. <span data-ttu-id="7acb6-134">Geben Sie in dem Feld **EK-Preis** den Betrag der Artikelgebühr an.</span><span class="sxs-lookup"><span data-stu-id="7acb6-134">In the **Direct Unit Cost** field, enter the amount of the item charge.</span></span>
7. <span data-ttu-id="7acb6-135">Füllen Sie die verbleibenden Felder je nach Bedarf aus.</span><span class="sxs-lookup"><span data-stu-id="7acb6-135">Fill in the remaining fields as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]

    <span data-ttu-id="7acb6-136">In den folgenden Schritten führen Sie die aktuelle Zuordnung aus.</span><span class="sxs-lookup"><span data-stu-id="7acb6-136">In the following steps, you will perform the actual assignment.</span></span> <span data-ttu-id="7acb6-137">Bis die Artikelgebühr vollständig zugewiesen wird, wird der Wert im Feld **Menge zuordnen** in roter Schrift angezeigt..</span><span class="sxs-lookup"><span data-stu-id="7acb6-137">Until the item charge is fully assigned, the value in the **Qty. to Assign** field is in red font.</span></span>
8. <span data-ttu-id="7acb6-138">Klicken Sie auf dem Inforegister **Zeilen** auf  Aktionen **Artikelgebühr-Zuweisung**.</span><span class="sxs-lookup"><span data-stu-id="7acb6-138">On the **Lines** tab, choose the **Item Charge Assignment** action.</span></span>

    <span data-ttu-id="7acb6-139">Das Fenster **Artikel Zu-/Abschlagszuweisung** öffnet sich und zeigt eine Zeile für jede Zeile der Art in der Einkaufsrechnung.</span><span class="sxs-lookup"><span data-stu-id="7acb6-139">The **Item Charge Assignment** window opens showing one line for each line of type Item on the purchase invoice.</span></span> <span data-ttu-id="7acb6-140">Um den Artikel Zu-/Abschlag in einen oder mehreren Verkaufsrechnungszeilen zuzuweisen, können Sie eine Funktion verwenden die es für Sie zugewiesen und verteilt oder Sie das **Menge. zuordnen** Feld manuell ausfüllen können.</span><span class="sxs-lookup"><span data-stu-id="7acb6-140">To assign the item charge to one or more invoice lines, you can use a function that assigns and distributes it for you or you can manually fill in the **Qty. to Assign** field.</span></span> <span data-ttu-id="7acb6-141">Die folgenden Schritte beschreiben, wie Vorschlagungs-ArtikelZu-/Abschlags-Zuweisungsfunktion verwendet.</span><span class="sxs-lookup"><span data-stu-id="7acb6-141">The following steps describe how to use the Suggest Item Charge Assignment function.</span></span>

9. <span data-ttu-id="7acb6-142">Im Fenster **Artikel Zu-/Abschlagszuweisung** wählen Sie die **Artikel Zu-/Abschlagszuweisung vorschlagen** Aktion aus.</span><span class="sxs-lookup"><span data-stu-id="7acb6-142">In the **Item Charge Assignment** window, choose the **Suggest Item Charge Assignment** action.</span></span>
10. <span data-ttu-id="7acb6-143">Wenn es mehr Rechnungszeilen als eine Art des Artikels gibt, wählen Sie eine der vier Verteilungsoptionen aus.</span><span class="sxs-lookup"><span data-stu-id="7acb6-143">If there are more than one invoice lines of type Item, choose one of the four distribution options.</span></span>  

<span data-ttu-id="7acb6-144">Bis die Artikelgebühr vollständig zugewiesen wird, wird der Wert im Feld **Menge zuordnen** in roter Schrift angezeigt..</span><span class="sxs-lookup"><span data-stu-id="7acb6-144">It the item charge is fully assigned, the value in the **Qty. to Assign** field on the purchase invoice is zero.</span></span>

<span data-ttu-id="7acb6-145">Der Artikelzuschlag wird nun der Einkaufsrechnung zugeordnet.</span><span class="sxs-lookup"><span data-stu-id="7acb6-145">The item charge is now assigned to the purchase invoice.</span></span> <span data-ttu-id="7acb6-146">Wenn Sie den Wareneingang der Einkaufsrechnung buchen, werden die Lagerwerte der Artikel mit den Kosten für Artikelzu-/-abschläge aktualisiert.</span><span class="sxs-lookup"><span data-stu-id="7acb6-146">When you post the receipt of the purchase invoice, the items' inventory values are updated with the cost of the item charge.</span></span>  

## <a name="to-assign-an-item-charge-from-a-separate-invoice-to-the-purchase-invoice-for-the-item"></a><span data-ttu-id="7acb6-147">Um einen Artikel Zu-/Abschlag in die Einkaufsrechnung für den Artikel zuordnen</span><span class="sxs-lookup"><span data-stu-id="7acb6-147">To assign an item charge from a separate invoice to the purchase invoice for the item</span></span>
<span data-ttu-id="7acb6-148">Wenn Sie eine Rechnung für die Zu-/Abschläge erhalten, nachdem Sie den Wareneingang der ursprünglichen Einkaufsrechnung wurde, gehen Sie folgendermaßen vor.</span><span class="sxs-lookup"><span data-stu-id="7acb6-148">If you received an invoice for the item charge after you posted the original purchase receipt, follow this procedure.</span></span>
1. <span data-ttu-id="7acb6-149">Wiederholen Sie die Schritte 1 bis 8 im ", um einen Artikel-Zu-/Abschlags in die Einkaufsrechnung für den Artikel zuzuordnen Abschnitt".</span><span class="sxs-lookup"><span data-stu-id="7acb6-149">Repeat steps 1 through 8 in the "To assign an item charge directly to the purchase invoice for the item" section.</span></span>
2. <span data-ttu-id="7acb6-150">Klicken Sie im Fenster  Artikel **Zu-/Abschlagszuweisung** auf  **Aktionen**,  Funktion,  Rücksendungszeilen holen.</span><span class="sxs-lookup"><span data-stu-id="7acb6-150">In the **Item Charge Assignment** window, choose the **Get Receipt Lines** action.</span></span>
3. <span data-ttu-id="7acb6-151">Im Fenster **Einkauf Lieferzeilen** wählen Sie die Zeile Geb. Einkaufslieferung für den Artikel, dem Sie den Artikel Zu-/Abschlag zuordnen möchten, und wählen Sie dann die Schaltfläche **OK** aus.</span><span class="sxs-lookup"><span data-stu-id="7acb6-151">In the **Purch. Receipt Lines** window, select the posted purchase receipt for the item that you want to assign the item charge to, and then choose the **OK** button.</span></span>
4. <span data-ttu-id="7acb6-152">Wählen Sie die **Artikel Zu-/Abschlagszuweisung vorschlagen** Aktion aus.</span><span class="sxs-lookup"><span data-stu-id="7acb6-152">Choose the **Suggest Item Charge Assignment** action.</span></span>

<span data-ttu-id="7acb6-153">Artikelzu-/Abschläge der separaten Einkaufsrechnung wird jetzt dem Artikel in der gebuchten Einkaufslieferung zugeordnet, d aktualisiert der Lagerwert des Artikels mit den Kosten für Artikelzu-/-abschläge.</span><span class="sxs-lookup"><span data-stu-id="7acb6-153">The item charge on the separate purchase invoice is now assigned to the item on the posted purchase receipt, thereby updating the item's inventory value with the cost of the item charge.</span></span>

## <a name="see-also"></a><span data-ttu-id="7acb6-154">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="7acb6-154">See Also</span></span>
[<span data-ttu-id="7acb6-155">Verwalten von Verbindlichkeiten</span><span class="sxs-lookup"><span data-stu-id="7acb6-155">Managing Payables</span></span>](payables-manage-payables.md)  
[<span data-ttu-id="7acb6-156">Erfassen eines Einkaufs</span><span class="sxs-lookup"><span data-stu-id="7acb6-156">Record Purchases</span></span>](purchasing-how-record-purchases.md)  
[<span data-ttu-id="7acb6-157">Verkaufsrechnung</span><span class="sxs-lookup"><span data-stu-id="7acb6-157">Invoice Sales</span></span>](sales-how-invoice-sales.md)  
<span data-ttu-id="7acb6-158">[Arbeiten mit [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="7acb6-158">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>  
