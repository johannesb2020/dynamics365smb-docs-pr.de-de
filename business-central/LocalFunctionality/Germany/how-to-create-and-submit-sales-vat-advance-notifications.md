---
title: Vorgehensweise beim Erstellen und Senden von Umsatzsteuervoranmeldungen
description: "In Business Central können Sie die Umsatzsteuervoranmeldungsdatei elektronisch an das ELSTER-Portal übermitteln. Sie können die Umsatzsteuervoranmeldungsdatei elektronisch an das Finanzamt übertragen, nachdem Sie den errechneten Steuerbetrag und die Bemessungsgrundlage geprüft haben."
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 07/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: d7fb34e1c9428a64c71ff47be8bcff174649c00d
ms.openlocfilehash: c1427e13f6a42b4b5ff3a192f91b0c76161cc673
ms.contentlocale: de-de
ms.lasthandoff: 03/22/2018

---
# <a name="create-and-submit-sales-vat-advance-notifications"></a><span data-ttu-id="d76c3-104">Gewusst wie: Erstellen und Senden von Umsatzsteuervoranmeldungen</span><span class="sxs-lookup"><span data-stu-id="d76c3-104">Create and Submit Sales VAT Advance Notifications</span></span>
<span data-ttu-id="d76c3-105">In [!INCLUDE[d365fin](../../includes/d365fin_md.md)] können Sie die Umsatzsteuervoranmeldungsdatei elektronisch an das ELSTER-Portal übermitteln.</span><span class="sxs-lookup"><span data-stu-id="d76c3-105">In [!INCLUDE[d365fin](../../includes/d365fin_md.md)], you can submit the sales VAT advance notification file electronically to the ELSTER portal.</span></span> <span data-ttu-id="d76c3-106">Sie können die Umsatzsteuervoranmeldungsdatei elektronisch an das Finanzamt übertragen, nachdem Sie den errechneten Steuerbetrag und die Bemessungsgrundlage geprüft haben.</span><span class="sxs-lookup"><span data-stu-id="d76c3-106">You can transmit the sales VAT advance notification file to the tax authorities after you have verified the calculated tax amount and the base amount.</span></span>  

## <a name="to-create-an-xml-document-for-sales-vat-advance-notification"></a><span data-ttu-id="d76c3-107">So erstellen Sie ein XML-Dokument für Umsatzsteuervoranmeldung</span><span class="sxs-lookup"><span data-stu-id="d76c3-107">To create an XML document for sales VAT advance notification</span></span>  

1.  <span data-ttu-id="d76c3-108">Wählen Sie das Symbol ![Nach Seite oder Bericht suchen](../../media/ui-search/search_small.png "Symbol „Nach Seite oder Bericht suchen”") aus, und geben Sie **Umsatzsteuervoranmeldungsliste** ein. Wählen Sie dann den zugehörigen Link aus.</span><span class="sxs-lookup"><span data-stu-id="d76c3-108">Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Sales Vat Advanced Notification List**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="d76c3-109">Im Fenster **Umsatzsteuervoranmeldungsliste** auf der Registerkarte Aktionen, wählen Sie **Neu** aus.</span><span class="sxs-lookup"><span data-stu-id="d76c3-109">In the **Sales Vat Advanced Notification List** window, choose the **New** action.</span></span>  
3.  <span data-ttu-id="d76c3-110">Füllen Sie im Fenster **USt.-Voranmeldungskarte** die Felder gemäß der Beschreibung in der folgenden Tabelle aus.</span><span class="sxs-lookup"><span data-stu-id="d76c3-110">In the **Sales VAT Adv. Notif. Card** window, fill in the fields as described in the following table.</span></span>  

    |<span data-ttu-id="d76c3-111">Feld</span><span class="sxs-lookup"><span data-stu-id="d76c3-111">Field</span></span>|<span data-ttu-id="d76c3-112">Description</span><span class="sxs-lookup"><span data-stu-id="d76c3-112">Description</span></span>|  
    |------------------------------------|---------------------------------------|  
    |<span data-ttu-id="d76c3-113">**Ansprechpartner für Finanzamt**</span><span class="sxs-lookup"><span data-stu-id="d76c3-113">**Contact for Tax Office**</span></span>|<span data-ttu-id="d76c3-114">Die Kontaktperson für das Finanzamt in Ihrer Organisation.</span><span class="sxs-lookup"><span data-stu-id="d76c3-114">The contact person for the tax office in your organization.</span></span>|  
    |<span data-ttu-id="d76c3-115">**Telefonnummer Kontakt**</span><span class="sxs-lookup"><span data-stu-id="d76c3-115">**Contact Phone No.**</span></span>|<span data-ttu-id="d76c3-116">Telefonnummer der Kontaktperson.</span><span class="sxs-lookup"><span data-stu-id="d76c3-116">The contact person's telephone number.</span></span>|  
    |<span data-ttu-id="d76c3-117">**Kontakt-E-Mail**</span><span class="sxs-lookup"><span data-stu-id="d76c3-117">**Contact E-Mail**</span></span>|<span data-ttu-id="d76c3-118">E-Mail-Adresse der Kontaktperson.</span><span class="sxs-lookup"><span data-stu-id="d76c3-118">The contact person's email address.</span></span>|  

5.  <span data-ttu-id="d76c3-119">Wählen Sie die Aktion **XML-Datei erstellen** aus.</span><span class="sxs-lookup"><span data-stu-id="d76c3-119">Choose the **Create XML-File** action.</span></span>  
6.  <span data-ttu-id="d76c3-120">Im Batchauftrag **MwSt.-Voranmeldung erstellen** im Inforegister **Optionen**, im Feld **XML-Datei**, wählen Sie **Erstellen** oder **Erstellen und anzeigen** aus.</span><span class="sxs-lookup"><span data-stu-id="d76c3-120">In the **Create Sales VAT Adv. Notif.** batch job, on the **Options** FastTab, in the **XML-File** field, select the **Create** or the **Create and Show** option.</span></span>  
7.  <span data-ttu-id="d76c3-121">Wählen Sie die Schaltfläche **OK** aus.</span><span class="sxs-lookup"><span data-stu-id="d76c3-121">Choose the **OK** button.</span></span>  

## <a name="to-submit-an-xml-document-for-sales-vat-advance-notification"></a><span data-ttu-id="d76c3-122">So übermitteln Sie ein XML-Dokument für Umsatzsteuervoranmeldung</span><span class="sxs-lookup"><span data-stu-id="d76c3-122">To submit an XML document for sales VAT advance notification</span></span>  

1.  <span data-ttu-id="d76c3-123">Im Fenster **Umsatzsteuervoranmeldungsliste** wählen Sie den Beleg aus, den Sie an ELSTER senden möchten.</span><span class="sxs-lookup"><span data-stu-id="d76c3-123">In the **Sales VAT Advance Notification List** window, select the document that you want to submit to ELSTER.</span></span>  
2.  <span data-ttu-id="d76c3-124">Wählen Sie die Aktion **XML-Datei übermitteln** aus.</span><span class="sxs-lookup"><span data-stu-id="d76c3-124">Choose the **Transmit XML-File** action.</span></span>  

<span data-ttu-id="d76c3-125">Die XML-Datei wird an ELSTER übermittelt.</span><span class="sxs-lookup"><span data-stu-id="d76c3-125">The XML file is transmitted to ELSTER.</span></span>  

## <a name="see-also"></a><span data-ttu-id="d76c3-126">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="d76c3-126">See Also</span></span>  
 <span data-ttu-id="d76c3-127">[Elektronische Übermittlung der Umsatzsteuervoranmeldungen an ELSTER](electronic-submission-of-sales-vat-advance-notifications-to-elster.md) </span><span class="sxs-lookup"><span data-stu-id="d76c3-127">[Electronic Submission of Sales VAT Advance Notifications to ELSTER](electronic-submission-of-sales-vat-advance-notifications-to-elster.md) </span></span>  
 [<span data-ttu-id="d76c3-128">Gewusst wie: Einrichten von Umsatzsteuervoranmeldungen für ELSTER</span><span class="sxs-lookup"><span data-stu-id="d76c3-128">Set Up Sales VAT Advance Notifications for ELSTER</span></span>](how-to-set-up-sales-vat-advance-notifications-for-elster.md)
