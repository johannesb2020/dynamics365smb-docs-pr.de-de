---
title: Vorgehensweise beim Korrigieren von MwSt.-Berichten
description: "Wenn Sie einen Korrektur-MwSt-Bericht übermitteln müssen oder einen übermittelten MwSt-Bericht löschen müssen, müssen Sie einen neuen MwSt-Bericht erstellen. Entsprechend der Gesetzgebung muss ein Korrekturbericht innerhalb eines Monats nach dem ursprünglichen Bericht übermittelt werden."
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 07/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: b34f276a764f0e828fbc1f015429df9852242a4c
ms.openlocfilehash: 76ab3e047f90e206316656b0a3c7907e905cb61c
ms.contentlocale: de-de
ms.lasthandoff: 03/22/2018

---
# <a name="correct-vat-reports"></a><span data-ttu-id="05f30-104">Zu korrigierender MwSt.-Bericht</span><span class="sxs-lookup"><span data-stu-id="05f30-104">Correct VAT Reports</span></span>
<span data-ttu-id="05f30-105">Wenn Sie einen Korrektur-MwSt-Bericht übermitteln müssen oder einen übermittelten MwSt-Bericht löschen müssen, müssen Sie einen neuen MwSt-Bericht erstellen.</span><span class="sxs-lookup"><span data-stu-id="05f30-105">If you have to submit a corrective VAT report or delete a submitted VAT report, you must create a new VAT report.</span></span> <span data-ttu-id="05f30-106">Entsprechend der Gesetzgebung muss ein Korrekturbericht innerhalb eines Monats nach dem ursprünglichen Bericht übermittelt werden.</span><span class="sxs-lookup"><span data-stu-id="05f30-106">According to the legislation, a corrective report must be submitted within a month of the initial report.</span></span>  

<span data-ttu-id="05f30-107">Wenn Sie einen Korrekturbericht erstellen, enthält die Erklärung zwei Zeilenarten pro korrigierter Zeile.</span><span class="sxs-lookup"><span data-stu-id="05f30-107">When you create a corrective report, the report will contain two line types per corrected line.</span></span> <span data-ttu-id="05f30-108">In einer Zeilenart, „Stornierung”, wird der Basiswert der MwSt. als Stornierung aufgezeichnet.</span><span class="sxs-lookup"><span data-stu-id="05f30-108">In one line type, Cancellation, the base value of the VAT is reported as a cancellation.</span></span> <span data-ttu-id="05f30-109">Alle anderen Informationen bleiben dieselben und können nicht bearbeitet werden.</span><span class="sxs-lookup"><span data-stu-id="05f30-109">All other information remains the same, and cannot be edited.</span></span> <span data-ttu-id="05f30-110">In einer neuen Zeile, Korrekturtyp, können Sie nach Bedarf Korrekturen am MwSt.-Betrag vornehmen.</span><span class="sxs-lookup"><span data-stu-id="05f30-110">On a new line, Correction type, you can make corrections as needed to the VAT amount.</span></span> <span data-ttu-id="05f30-111">Bei der Aktion **Zeilen vorschlagen** wird jedoch der richtige Betrag, basierend auf den Filtern und gebuchten Belegen, vorgeschlagen.</span><span class="sxs-lookup"><span data-stu-id="05f30-111">The **Suggest Lines** action, however, will suggest the correct amount based on the filters and posted documents.</span></span> <span data-ttu-id="05f30-112">Sie können die **USt-IdNr.** nicht korrigieren oder ändern. Jede Periode, die korrigiert wird, benötigt ihren eigenen Korrekturbericht.</span><span class="sxs-lookup"><span data-stu-id="05f30-112">You cannot correct or modify the **VAT Registration No.** Each period being corrected needs its own corrective report.</span></span>  

<span data-ttu-id="05f30-113">Bei der Aktion **Zeilen vorschlagen**, werden die zu meldenden Werte neu berechnet.</span><span class="sxs-lookup"><span data-stu-id="05f30-113">The **Suggest Lines** action recalculates the values to report.</span></span> <span data-ttu-id="05f30-114">Die Aktion **Zeilen korrigieren** wird verwendet, um manuelle Änderungen vorzunehmen.</span><span class="sxs-lookup"><span data-stu-id="05f30-114">The **Correct Lines** action is used to make manual changes.</span></span> <span data-ttu-id="05f30-115">Sie können die Auswirkungen der zwei Aktionen kombinieren, um den Bericht zu korrigieren.</span><span class="sxs-lookup"><span data-stu-id="05f30-115">You can combine the effects of the two actions to correct your report.</span></span>  

<span data-ttu-id="05f30-116">**Beispielkorrekturszenarien**</span><span class="sxs-lookup"><span data-stu-id="05f30-116">**Example corrections scenarios**</span></span>  

1.  <span data-ttu-id="05f30-117">Wenn Sie zusätzliche MwSt-Posten buchen, nachdem Sie den Standardbericht im Berichtszeitraum übermitteln, wählen Sie **Zeilen vorschlagen** in der Gruppe **Verarbeiten** aus, um die aktualisierten Beträge zu erhalten.</span><span class="sxs-lookup"><span data-stu-id="05f30-117">If you post additional VAT entries after you submit the Standard report in the report period, choose **Suggest Lines** in the **Process** group to get the updated amounts.</span></span>  

    > [!NOTE]  
    >  <span data-ttu-id="05f30-118">Wenn Sie den Betrag für einen Debitor oder Keditor manuell geändert haben, wird dieser Betrag überschrieben, wenn zusätzliche MwSt-Posten gebucht werden.</span><span class="sxs-lookup"><span data-stu-id="05f30-118">If you manually changed the amount for a customer or vendor, this amount will be overwritten when additional VAT entries are posted.</span></span> <span data-ttu-id="05f30-119">Aktualisieren Sie den Betrag entsprechend.</span><span class="sxs-lookup"><span data-stu-id="05f30-119">Update the amount accordingly.</span></span>  

2.  <span data-ttu-id="05f30-120">Wenn Sie den Betrag einer Berichtszeile ändern möchten, die bereits übermittelt wurde und keine neuen MwSt-Posten gebucht werden, wählen Sie **Zeilen korrigieren** in der Gruppe Verarbeiten aus.</span><span class="sxs-lookup"><span data-stu-id="05f30-120">If you want to change the amount of a report line that has already been submitted and no new VAT entries are posted, choose the  **Correct Lines** action.</span></span> <span data-ttu-id="05f30-121">Wählen Sie im Fenster **MwST-Berichtszeilen** die zu korrigierenden Lieferzeilen aus, und klicken Sie auf **OK**.</span><span class="sxs-lookup"><span data-stu-id="05f30-121">In the **VAT Report Lines** window, select the lines that you want to correct, and then choose the **OK** button.</span></span>  

    <span data-ttu-id="05f30-122">Für jeden Posten werden zwei Zeilen angezeigt: Stornierung oder Korrektur.</span><span class="sxs-lookup"><span data-stu-id="05f30-122">For each entry, two lines are displayed: Cancellation and Correction.</span></span> <span data-ttu-id="05f30-123">Sie können jetzt den Betrag der Korrekturzeile ändern.</span><span class="sxs-lookup"><span data-stu-id="05f30-123">You can now change the amount on the Correction line.</span></span>  

    > [!NOTE]  
    >  <span data-ttu-id="05f30-124">Die Aktion **Zeilen korrigieren** schlägt den Betrag nicht vor, der auf MwSt-Posten basiert.</span><span class="sxs-lookup"><span data-stu-id="05f30-124">The **Correct Lines** action will not suggest the amount based in VAT entries.</span></span> <span data-ttu-id="05f30-125">Wenn Sie neue MwSt-Posten für den Debitor oder Kreditor haben, verwenden Sie stattdessen **Zeilen vorschlagen**.</span><span class="sxs-lookup"><span data-stu-id="05f30-125">If you have new VAT entries for the customer or vendor, instead use the **Suggest Lines** action.</span></span>  

3.  <span data-ttu-id="05f30-126">Wenn Sie die falschen Filter verwendet haben, wie beispielsweise die falsche MwSt-Produktbuchungsgruppe, wählen Sie **Zeilen vorschlagen** in der Gruppe Verarbeiten aus, und legen Sie dann die Filter nach Bedarf fest.</span><span class="sxs-lookup"><span data-stu-id="05f30-126">If you used the wrong filters, for example, the wrong VAT product posting group, choose the **Suggest Lines** action, and then set filters as needed.</span></span>  

    <span data-ttu-id="05f30-127">**Zeilen vorschlagen** erstellt Posten, um die Differenz zwischen den Filter zu widerzuspiegeln.</span><span class="sxs-lookup"><span data-stu-id="05f30-127">**Suggest Lines** will create entries to account for the difference between the filters.</span></span>  

    > [!NOTE]  
    >  <span data-ttu-id="05f30-128">Wenn die aktualisierten Filter einen Debitor oder einen Kreditor ausschließen, erstellt [!INCLUDE[d365fin](../../includes/d365fin_md.md)] eine Stornierungszeile für den vorherigen berichteten Betrag und einen Korrekturposten mit Betrag 0.</span><span class="sxs-lookup"><span data-stu-id="05f30-128">If the updated filters exclude a customer or vendor, [!INCLUDE[d365fin](../../includes/d365fin_md.md)] creates a Cancellation line for the previous reported amount and a Correction entry with amount 0.</span></span>

## <a name="to-correct-a-vat-report"></a><span data-ttu-id="05f30-129">So wird ein MwSt-Bericht korrigiert</span><span class="sxs-lookup"><span data-stu-id="05f30-129">To correct a VAT report</span></span>  

1.  <span data-ttu-id="05f30-130">Erstellen Sie einen neuen MwSt-Bericht.</span><span class="sxs-lookup"><span data-stu-id="05f30-130">Create a new VAT report.</span></span> <span data-ttu-id="05f30-131">Weitere Informationen finden Sie unter [MwSt-Berichte erstellen](how-to-create-vat-reports.md).</span><span class="sxs-lookup"><span data-stu-id="05f30-131">For more information, see [Create VAT Reports](how-to-create-vat-reports.md).</span></span>  
2.  <span data-ttu-id="05f30-132">Füllen Sie die Felder im Inforegister **Allgemein** aus, und legen Sie das Feld **MwSt-Berichtstyp** auf „Korrigiert” fest.</span><span class="sxs-lookup"><span data-stu-id="05f30-132">Fill in the fields in the **General** FastTab, and set the **VAT Report Type** field to Corrective.</span></span>  
3.  <span data-ttu-id="05f30-133">In der **Originalberichtsnr.**</span><span class="sxs-lookup"><span data-stu-id="05f30-133">In the **Original Report No.**</span></span> <span data-ttu-id="05f30-134">Feld, wählen Sie den Bericht aus, die Sie korrigieren möchten.</span><span class="sxs-lookup"><span data-stu-id="05f30-134">field, select the report that you want to correct.</span></span> <span data-ttu-id="05f30-135">Sie können nur Berichte vom Typ „Standard” auswählen, die als „Übermittelt” markiert sind.</span><span class="sxs-lookup"><span data-stu-id="05f30-135">You can only select reports of type Standard that have been marked as Submitted.</span></span>  
4.  <span data-ttu-id="05f30-136">Erstellen Sie Ihre Korrektur-MwSt-Berichts-Zeilenposten.</span><span class="sxs-lookup"><span data-stu-id="05f30-136">Create your correction VAT report line entries.</span></span>  

    <span data-ttu-id="05f30-137">Wählen Sie die Aktion **Mahnungszeile vorschlagen**.</span><span class="sxs-lookup"><span data-stu-id="05f30-137">Choose the **Suggest Lines** action.</span></span> <span data-ttu-id="05f30-138">Legen Sie die Filter gemäß Bedarf fest.</span><span class="sxs-lookup"><span data-stu-id="05f30-138">Set filters as needed.</span></span>  

    <span data-ttu-id="05f30-139">In jeder Zeile können Sie einen Drilldown zu den Beträgen durchführen, um anzuzeigen, aus welchen MwSt-Posten sich der Betrag zusammensetzt.</span><span class="sxs-lookup"><span data-stu-id="05f30-139">On each line you can drill down on the amounts to see which VAT entries make up the amount.</span></span> <span data-ttu-id="05f30-140">Ändern Sie den Betrag nach Bedarf.</span><span class="sxs-lookup"><span data-stu-id="05f30-140">Change the amount if needed.</span></span> <span data-ttu-id="05f30-141">Sie können die **USt-IdNr.** jedoch nicht bearbeiten.</span><span class="sxs-lookup"><span data-stu-id="05f30-141">You cannot edit, however, the **VAT Registration No.**.</span></span>  

5.  <span data-ttu-id="05f30-142">Wenn die **Vorschlagszeilen** Aktion keine Vorschläge bietet, die Beträge zu korrigieren, die erforderlich sind, verwenden Sie die Aktion**Zeilen korrigieren**, um Stornierungs- und Korrekturzeilen für den Debitor oder Kreditor einzufügen.</span><span class="sxs-lookup"><span data-stu-id="05f30-142">If the **Suggest Lines** action does not provide suggestions to correct the amounts that you intended, use the **Correct Lines** action to insert cancellation and correction lines for the customer or vendor.</span></span>  
6.  <span data-ttu-id="05f30-143">Fahren Sie mit dem MwSt-Berichterstellungsprozess fort und geben Sie den Bericht frei.</span><span class="sxs-lookup"><span data-stu-id="05f30-143">Continue with the VAT report creation process, and release the report.</span></span>  

## <a name="see-also"></a><span data-ttu-id="05f30-144">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="05f30-144">See Also</span></span>  
 [<span data-ttu-id="05f30-145">Richten Sie die MwSt.-Berichte ein.</span><span class="sxs-lookup"><span data-stu-id="05f30-145">Set Up VAT Reports</span></span>](how-to-set-up-vat-reports.md)
