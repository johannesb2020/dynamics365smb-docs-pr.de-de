---
title: Abschreibungsmethoden einrichten| Microsoft Docs
description: "Sie geben in einem AfA-Buch an, wie Sie Anlagen abschreiben oder anzeigen möchten."
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: write down
ms.date: 06/02/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: e7dcdc0935a8793ae226dfc2f9709b5b8f487a62
ms.openlocfilehash: 01f094c5325773b2c4e9675412fce7d7a29449bd
ms.contentlocale: de-de
ms.lasthandoff: 03/22/2018

---
# <a name="set-up-fixed-asset-depreciation"></a><span data-ttu-id="996b7-103">Richten Sie eine neue Anlagenkarte ein</span><span class="sxs-lookup"><span data-stu-id="996b7-103">Set Up Fixed Asset Depreciation</span></span>
 <span data-ttu-id="996b7-104">Sie können unterschiedliche Abschreibungsmethoden für Bilanzen und Steuern verwenden.</span><span class="sxs-lookup"><span data-stu-id="996b7-104">You can use various methods of depreciation for preparing financial statements and income tax returns.</span></span> <span data-ttu-id="996b7-105">Viele Großunternehmen verwenden die lineare Abschreibung in ihren Bilanzen, da dadurch im Allgemeinen höhere Gewinne ausgewiesen werden können.</span><span class="sxs-lookup"><span data-stu-id="996b7-105">Many large corporations use straight-line depreciation in their financial statements because this generally permits reporting higher earnings.</span></span> <span data-ttu-id="996b7-106">Für steuerliche Zwecke verwenden viele Unternehmen beschleunigte Abschreibungsmethoden.</span><span class="sxs-lookup"><span data-stu-id="996b7-106">For income tax purposes, however, many businesses use an accelerated depreciation method.</span></span> <span data-ttu-id="996b7-107">Weitere Informationen finden Sie unter [AfA-Methoden](fa-depreciation-methods.md).</span><span class="sxs-lookup"><span data-stu-id="996b7-107">For more information, see [Depreciation Methods](fa-depreciation-methods.md).</span></span>

 <span data-ttu-id="996b7-108">Nachdem Sie die erforderlichen AfA-Bücher erstellt haben, müssen Sie jeder Anlage mindestens ein AfA-Buch zuweisen.</span><span class="sxs-lookup"><span data-stu-id="996b7-108">When you have created the relevant depreciation books, you must assign one or more depreciation books to each fixed asset.</span></span> <span data-ttu-id="996b7-109">Ein AfA-Buch, das einer Anlage zugewiesen ist, wird als Anlagen-AfA-Buch bezeichnet.</span><span class="sxs-lookup"><span data-stu-id="996b7-109">A depreciation book that is assigned to a fixed asset is referred to as a fixed asset depreciation book.</span></span> <span data-ttu-id="996b7-110">Entsprechend wird das Fenster für zugewiesene AfA-Bücher **Anlagen-AfA-Bücher** genannt.</span><span class="sxs-lookup"><span data-stu-id="996b7-110">Accordingly, the window for assigned depreciation books is called **FA Depreciation Books**.</span></span>

## <a name="to-create-a-depreciation-book"></a><span data-ttu-id="996b7-111">So erstellen Sie ein Anlagen-AfA-Buch</span><span class="sxs-lookup"><span data-stu-id="996b7-111">To create a depreciation book</span></span>
<span data-ttu-id="996b7-112">In einem AfA-Buch können Sie festlegen, wie eine Anlage abgeschrieben wird.</span><span class="sxs-lookup"><span data-stu-id="996b7-112">In a fixed asset depreciation book, you specify how fixed assets are depreciated.</span></span> <span data-ttu-id="996b7-113">Sie können mehrere AfA-Bücher einrichten, um die verschiedenen Abschreibungsarten zu erleichtern.</span><span class="sxs-lookup"><span data-stu-id="996b7-113">To accommodate various methods of depreciation, you can set up multiple depreciation books.</span></span>  

1. <span data-ttu-id="996b7-114">Wählen Sie in der rechten oberen Ecke ![Nach Seite oder Bericht suchen](media/ui-search/search_small.png "Symbol Nach Seite oder Bericht suchen") und geben **AfA-Buchliste** ein. Wählen Sie dann den zugehörigen Link aus.</span><span class="sxs-lookup"><span data-stu-id="996b7-114">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Depreciation Books**, and then choose the related link.</span></span>
2. <span data-ttu-id="996b7-115">Im Feld **AfA-Bücher Übersicht** wählen Sie die Aktion **Neu** aus.</span><span class="sxs-lookup"><span data-stu-id="996b7-115">In the **Depreciation Books List** window, choose the **New** action.</span></span>
3. <span data-ttu-id="996b7-116">Füllen Sie im Fenster **AfA-Buch-Karte** die Felder nach Bedarf aus.</span><span class="sxs-lookup"><span data-stu-id="996b7-116">In the **Depreciation Book Card** window, fill in the fields as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]

    > [!NOTE]  
    >   <span data-ttu-id="996b7-117">Hinweis: Sie können Anlagentransaktionen im Fenster **Anlagen Fibu Buch.-Blatt** oder im Fenster **Anlagen Buch - Blatt** erfassen, abhängig davon, ob die Transaktionen für Finanzberichte oder zur internen Verwaltung bestimmt sind.</span><span class="sxs-lookup"><span data-stu-id="996b7-117">You can record fixed asset transactions in the **Fixed Asset G/L Journal** window or in the **Fixed Asset Journal** window, depending on whether the transactions are for financial reporting or for internal management.</span></span> <span data-ttu-id="996b7-118">Führen Sie den nächsten Schritt aus, um festzulegen, welche Art von Buch.-Blatt für die verschiedenen Anlagenaktivitäten standardmäßig verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="996b7-118">Follow the next step to define which type of journal is used for the different fixed asset activities by default.</span></span>
4. <span data-ttu-id="996b7-119">Aktivieren Sie im Inforregister **Integration** das Kontrollkästchen für jede Anlagenaktivität, deren Transaktionen Sie mithilfe des Fensters **Anlagen Fibu Buch.-Blatt** buchen möchten.</span><span class="sxs-lookup"><span data-stu-id="996b7-119">On the **Integration** FastTab, select the check box for each fixed asset activity whose transactions you want to post using the **Fixed Asset G/L Journal** window.</span></span>
5. <span data-ttu-id="996b7-120">Wiederholen Sie die Schritte 2 bis 4 für jede AfA- oder Buchungsmethode, die Sie den Anlagen als AfA-Buch zuweisen möchten.</span><span class="sxs-lookup"><span data-stu-id="996b7-120">Repeat steps 2 through 4 for each depreciation method or posting method that you want to assign to fixed assets as a depreciation book.</span></span>

## <a name="to-assign-a-depreciation-book-to-a-fixed-asset"></a><span data-ttu-id="996b7-121">So verknüpfen Sie ein AfA-Buchs mit einer Anlage</span><span class="sxs-lookup"><span data-stu-id="996b7-121">To assign a depreciation book to a fixed asset</span></span>
1. <span data-ttu-id="996b7-122">Wählen Sie in der rechten oberen Ecke das Symbol ![Nach Seite oder Bericht suchen](media/ui-search/search_small.png "Nach Seite oder Bericht suchen") und geben **Anlagen** ein. Wählen Sie dann den zugehörigen Link aus.</span><span class="sxs-lookup"><span data-stu-id="996b7-122">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Fixed Assets**, and then choose the related link.</span></span>
2. <span data-ttu-id="996b7-123">Wählen Sie die Anlage aus, für die Sie ein Anlagen-AfA-Buch einrichten möchten.</span><span class="sxs-lookup"><span data-stu-id="996b7-123">Select the fixed asset that you want to set up a fixed asset depreciation book for.</span></span>
3. <span data-ttu-id="996b7-124">Füllen Sie im Inforegister **AfA-Buch** die Felder nach Bedarf aus.</span><span class="sxs-lookup"><span data-stu-id="996b7-124">On the **Depreciation Book** FastTab, fill in the fields as necessary.</span></span>
4. <span data-ttu-id="996b7-125">Wenn Sie mehrere AfA-Bücher der Anlage zuweisen müssen, wählen Sie die Aktion **Weitere AfA-Bücher hinzufügen** aus.</span><span class="sxs-lookup"><span data-stu-id="996b7-125">If you need to assign more than one depreciation book to the fixed asset, choose the **Add More Depreciation Books** action.</span></span>
5. <span data-ttu-id="996b7-126">Wählen Sie die Aktion **AfA-Bücher** aus , um eine oder mehrere Anlagen-AfA-Bücher anzugeben.</span><span class="sxs-lookup"><span data-stu-id="996b7-126">Alternatively, choose the **Depreciation Books** action to specify one or more fixed asset depreciation books.</span></span>

    > [!NOTE]  
    >   <span data-ttu-id="996b7-127">Hinweis: Wenn Sie die manuelle AfA-Methode verwenden, müssen Sie die Abschreibung manuell im Anlagen Fibu Buch.-Blatt eingeben.</span><span class="sxs-lookup"><span data-stu-id="996b7-127">When you use the manual depreciation method, you must enter depreciation manually in the fixed asset G/L journal.</span></span> <span data-ttu-id="996b7-128">Die Funktion **AfA berechnen** berücksichtigt keine Anlagen mit der AfA-Methode "Manuell".</span><span class="sxs-lookup"><span data-stu-id="996b7-128">The **Calculate Depreciation** function omits fixed assets that use the manual depreciation method.</span></span> <span data-ttu-id="996b7-129">Sie können diese Methode für Anlagen verwenden, die nicht abgeschrieben werden, wie z. B. Land.</span><span class="sxs-lookup"><span data-stu-id="996b7-129">You can use this method for assets that are not subject to depreciation, such as land.</span></span>

## <a name="to-assign-a-depreciation-book-to-multiple-fixed-assets-with-a-batch-job"></a><span data-ttu-id="996b7-130">So weisen Sie ein AfA-Buch mehreren Anlagen mit einer Stapelverarbeitung zu</span><span class="sxs-lookup"><span data-stu-id="996b7-130">To assign a depreciation book to multiple fixed assets with a batch job</span></span>
<span data-ttu-id="996b7-131">Falls Sie ein AfA-Buch mit mehreren Anlagen verknüpfen möchten, können Sie die Stapelverarbeitung **Anlagen-AfA-Buch erstellen** verwenden, um die Anwendung die erforderlichen AfA-Bücher automatisch erstellen zu lassen.</span><span class="sxs-lookup"><span data-stu-id="996b7-131">If you want to assign a depreciation book to several fixed assets, you can use the **Create FA Depreciation Books** batch job to create fixed asset depreciation books.</span></span>  

1. <span data-ttu-id="996b7-132">Wählen Sie in der rechten oberen Ecke das Symbol ![Nach Seite oder Bericht suchen](media/ui-search/search_small.png "Nach Seite oder Bericht suchen") und geben **Anlagen** ein. Wählen Sie dann den zugehörigen Link aus.</span><span class="sxs-lookup"><span data-stu-id="996b7-132">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Fixed Assets**, and then choose the related link.</span></span>
2. <span data-ttu-id="996b7-133">Wählen Sie die Anlage aus, die Sie einrichten möchten und der ein AfA-Buch zugewiesen werden soll, und wählen Sie dann die Aktion **Bearbeiten** aus.</span><span class="sxs-lookup"><span data-stu-id="996b7-133">Select the fixed asset that you want to set up a assign a depreciation book to, and then choose the **Edit** action.</span></span>
3. <span data-ttu-id="996b7-134">Wählen Sie im Fenster **AfA-Buch - Karte** die Aktion **Anlagen-AfA-Bücher erstellen** aus.</span><span class="sxs-lookup"><span data-stu-id="996b7-134">In the **Depreciation Book Card** window, choose the **Create FA Depreciation Books** action.</span></span>
4. <span data-ttu-id="996b7-135">Füllen Sie im Fenster **Anlagen-AfA-Buch erstellen** das Fenster **AfA-Buch** aus.</span><span class="sxs-lookup"><span data-stu-id="996b7-135">In the **Create FA Depreciation Books** window, fill in the **Depreciation Book** field.</span></span>
5. <span data-ttu-id="996b7-136">Klicken Sie im Feld **Kopieren von Anl.-Nr.** auf den AssistButton, und wählen Sie dann die Nummer der Anlage, die Sie als Basis für das neue AfA-Buch verwenden möchten.</span><span class="sxs-lookup"><span data-stu-id="996b7-136">Choose the **Copy from FA No.** field, and then select the fixed asset number that you want to use as the basis for creating new fixed asset depreciation books.</span></span>

    <span data-ttu-id="996b7-137">Wenn Sie dieses Feld ausfüllen, enthalten die Abschreibungsfelder in den neuen Anlagen-AfA-Büchern die gleichen Informationen wie die entsprechenden Felder im Anlagen-AfA-Buch, aus dem Sie kopieren.</span><span class="sxs-lookup"><span data-stu-id="996b7-137">If you fill in this field, the depreciation fields in the new fixed asset depreciation books will contain the same information as the corresponding fields in the fixed asset depreciation book that you copy from.</span></span> <span data-ttu-id="996b7-138">Lassen Sie dieses Feld leer, wenn Sie neue Anlagen-AfA-Bücher mit leeren Abschreibungsfeldern erstellen möchten.</span><span class="sxs-lookup"><span data-stu-id="996b7-138">Leave the field blank if you want to create new fixed asset depreciation books with empty depreciation fields.</span></span>  
6. <span data-ttu-id="996b7-139">Im Inforegister **Anlage** können Sie einen Filter setzen, um die Anlagen auszuwählen, für die Sie Anlagen-AfA-Bücher erstellen wollen.</span><span class="sxs-lookup"><span data-stu-id="996b7-139">On the **Fixed Asset** FastTab, you can set a filter to select the assets that you want to create the fixed asset depreciation books for.</span></span>
7. <span data-ttu-id="996b7-140">Wählen Sie die Schaltfläche **OK** aus.</span><span class="sxs-lookup"><span data-stu-id="996b7-140">Choose the **OK** button.</span></span>

## <a name="to-set-up-depreciation-posting-types"></a><span data-ttu-id="996b7-141">So richten Sie AfA-Buchungsarten ein:</span><span class="sxs-lookup"><span data-stu-id="996b7-141">To set up depreciation posting types</span></span>
<span data-ttu-id="996b7-142">Für jedes AfA-Buch müssen Sie festlegen, wie die verschiedenen Buchungsarten in [!INCLUDE[d365fin](includes/d365fin_md.md)] verarbeitet werden sollen.</span><span class="sxs-lookup"><span data-stu-id="996b7-142">For each depreciation book, you must set up how you want [!INCLUDE[d365fin](includes/d365fin_md.md)] to handle various posting types.</span></span> <span data-ttu-id="996b7-143">Beispielsweise ob Buchungen Soll- oder Habenposten sein sollen und ob die Buchungsart in der AfA-Grundlage enthalten sein soll.</span><span class="sxs-lookup"><span data-stu-id="996b7-143">For example, whether posting should be debit or credit and whether the posting type should be included in the depreciable basis.</span></span>  

1. <span data-ttu-id="996b7-144">Wählen Sie in der rechten oberen Ecke ![Nach Seite oder Bericht suchen](media/ui-search/search_small.png "Symbol Nach Seite oder Bericht suchen") und geben **AfA-Buchliste** ein. Wählen Sie dann den zugehörigen Link aus.</span><span class="sxs-lookup"><span data-stu-id="996b7-144">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Depreciation Books**, and then choose the related link.</span></span>  
2. <span data-ttu-id="996b7-145">Wählen Sie das AfA-Buch aus, die Sie einrichten möchten und wählen Sie dann die Aktion **Anlagenbuchungsart Einr.** aus.</span><span class="sxs-lookup"><span data-stu-id="996b7-145">Select the depreciation book that you want to set up, and them choose the **FA Posting Type Setup** action.</span></span>
3. <span data-ttu-id="996b7-146">Füllen Sie im Fenster **Anlagenbuchungsart Einr.** die notwendigen Felder aus.</span><span class="sxs-lookup"><span data-stu-id="996b7-146">In the **FA Posting Type Setup** window, fill in the fields as necessary.</span></span>

    > [!NOTE]  
    >   <span data-ttu-id="996b7-147">Sie können in dem Fenster **Anlagenbuchungsart Einr.** keine Zeilen löschen oder einfügen.</span><span class="sxs-lookup"><span data-stu-id="996b7-147">You cannot insert or delete lines in the **FA Posting Type Setup** window.</span></span> <span data-ttu-id="996b7-148">Sie können nur die bestehenden Zeilen ändern.</span><span class="sxs-lookup"><span data-stu-id="996b7-148">You can only modify the existing lines.</span></span>

<span data-ttu-id="996b7-149">Es wird empfohlen, die Einrichtung von AfA-Büchern, für die bereits Posten gebucht wurden, nicht zu ändern.</span><span class="sxs-lookup"><span data-stu-id="996b7-149">We recommend that you do not change the setup for depreciation books for entries that have already been posted.</span></span> <span data-ttu-id="996b7-150">Änderungen haben keinen Einfluss auf Posten, die bereits gebucht wurden, da andernfalls die Statistik für das AfA-Buch verfälscht würde.</span><span class="sxs-lookup"><span data-stu-id="996b7-150">Changes will not affect the entries that are already posted, which would make depreciation book statistics misleading.</span></span>

## <a name="to-set-up-default-templates-and-batches-for-fixed-asset-depreciation"></a><span data-ttu-id="996b7-151">So richten Sie Standardvorlagen und -Standardstapelverarbeitungen für Anlagen-AfA ein</span><span class="sxs-lookup"><span data-stu-id="996b7-151">To set up default templates and batches for fixed asset depreciation</span></span>
<span data-ttu-id="996b7-152">Sie können für jedes AfA-Buch Vorgaben für Vorlagen und Buch.-Blätter definieren.</span><span class="sxs-lookup"><span data-stu-id="996b7-152">For each depreciation book, you define a default setup of templates and batches.</span></span> <span data-ttu-id="996b7-153">Sie nutzen diese Standards, um Zeilen aus einem Buch.-Blatt in ein anderes zu kopieren, wenn die Batchaufträge **AfA berechnen** oder **Anlagen indexieren** Buch.-Blattzeilen erstellen oder wenn Anschaffungskosten im Versicherungs Buch.-Blatt doppelt vorhanden sind.</span><span class="sxs-lookup"><span data-stu-id="996b7-153">You use these defaults to duplicate lines from one journal to another, create journal lines using the **Calculate Depreciation** or **Index Fixed Assets** batch jobs, duplicate acquisition costs in the insurance journal.</span></span>  

1. <span data-ttu-id="996b7-154">Wählen Sie in der rechten oberen Ecke ![Nach Seite oder Bericht suchen](media/ui-search/search_small.png "Symbol Nach Seite oder Bericht suchen") und geben **AfA-Buchliste** ein. Wählen Sie dann den zugehörigen Link aus.</span><span class="sxs-lookup"><span data-stu-id="996b7-154">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Depreciation Books**, and then choose the related link.</span></span>  
2. <span data-ttu-id="996b7-155">Wählen Sie das AfA-Buch aus, für das Sie die Standardbuch.-Blätter festlegen möchten und wählen Sie dann die Aktion **Anlagen Buch.-Blatt Einr.** aus.</span><span class="sxs-lookup"><span data-stu-id="996b7-155">Select the depreciation book that you want to define default journals for, and then choose the **FA Journal Setup** action.</span></span>  
3. <span data-ttu-id="996b7-156">Falls Sie eine Standardeinrichtung für jeden einzelnen Benutzer definieren möchten, wählen Sie das Feld **Benutzer-ID** aus, um über das Fenster **Benutzer** auszuwählen.</span><span class="sxs-lookup"><span data-stu-id="996b7-156">If you want to have a default setup for each user, choose the **User ID** field to select from the **Users** window.</span></span>  
4. <span data-ttu-id="996b7-157">Wählen Sie in den anderen Feldern die Buch.-Blattvorlage oder den Buch.-Blattnamen, die standardmäßig verwendet werden müssen.</span><span class="sxs-lookup"><span data-stu-id="996b7-157">In the other fields, select the journal template or journal batch that must be used by default.</span></span>  

## <a name="see-also"></a><span data-ttu-id="996b7-158">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="996b7-158">See Also</span></span>
[<span data-ttu-id="996b7-159">Anlagen einrichten</span><span class="sxs-lookup"><span data-stu-id="996b7-159">Setting Up Fixed Assets</span></span>](fa-setup.md)  
[<span data-ttu-id="996b7-160">Anlagen</span><span class="sxs-lookup"><span data-stu-id="996b7-160">Fixed Assets</span></span>](fa-manage.md)  
[<span data-ttu-id="996b7-161">Finanzen</span><span class="sxs-lookup"><span data-stu-id="996b7-161">Finance</span></span>](finance.md)  
[<span data-ttu-id="996b7-162">Erste Schritte</span><span class="sxs-lookup"><span data-stu-id="996b7-162">Getting Started</span></span>](product-get-started.md)  
<span data-ttu-id="996b7-163">[Arbeiten mit [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="996b7-163">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>
