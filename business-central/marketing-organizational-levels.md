---
title: "Einrichten von Position für Kontaktpersonen| Microsoft Docs"
description: "Sie können Ihren Kontakten Positionen zuordnen, um zu bestimmen, welche Position sie innerhalb ihres Unternehmens innehaben (beispielsweise Topmanagement)."
services: project-madeira
documentationcenter: 
author: jswymer
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: relationship, client, prospect
ms.date: 06/06/2017
ms.author: jswymer
ms.translationtype: HT
ms.sourcegitcommit: d7fb34e1c9428a64c71ff47be8bcff174649c00d
ms.openlocfilehash: 974133ffb0324cf6bc3ed37436adb9fb237f5e4d
ms.contentlocale: de-de
ms.lasthandoff: 03/22/2018

---
# <a name="set-up-organizational-levels-for-contact-persons"></a><span data-ttu-id="0a96f-103">Einrichten von Position für Kontaktpersonen</span><span class="sxs-lookup"><span data-stu-id="0a96f-103">Set Up Organizational Levels for Contact Persons</span></span>
<span data-ttu-id="0a96f-104">Sie können Ihren Kontakten Positionen zuordnen, um zu bestimmen, welche Position sie innerhalb ihres Unternehmens innehaben (beispielsweise Topmanagement).</span><span class="sxs-lookup"><span data-stu-id="0a96f-104">You can use organizational levels on your contacts to specify which position they have in the company, for example, top management.</span></span> <span data-ttu-id="0a96f-105">Sie können diese Informationen nutzen, wenn Sie Informationen über Ihre Kontakte eingeben.</span><span class="sxs-lookup"><span data-stu-id="0a96f-105">You can use this information when entering information about your contacts.</span></span>

<span data-ttu-id="0a96f-106">Die Nutzung von Positionen zu Kontakten ist ein zwei Schritte umfassender Prozess.</span><span class="sxs-lookup"><span data-stu-id="0a96f-106">Using organizational levels on contacts is a two-step process.</span></span> <span data-ttu-id="0a96f-107">Zuerst definieren Sie den Positionscode.</span><span class="sxs-lookup"><span data-stu-id="0a96f-107">First, you define the organizational level code.</span></span> <span data-ttu-id="0a96f-108">Sie müssen diesen Schritt nur einmal für jede Position ausführen.</span><span class="sxs-lookup"><span data-stu-id="0a96f-108">You only have to perform this step one time for each organizational level.</span></span> <span data-ttu-id="0a96f-109">Sobald Sie einen Positionscode haben, können Sie den Code zu den Kontaktpersonen zuweisen.</span><span class="sxs-lookup"><span data-stu-id="0a96f-109">Once you have an organizational level code, you can start to assign the code to contact persons.</span></span>

## <a name="to-define-an-organizational-level-code"></a><span data-ttu-id="0a96f-110">Um einen Organisationsstufencode zu definieren</span><span class="sxs-lookup"><span data-stu-id="0a96f-110">To define an organizational level code</span></span>
<span data-ttu-id="0a96f-111">Der Positionscode definiert die Art oder die Kategorie der Position (z. B. CEO oder CFO).</span><span class="sxs-lookup"><span data-stu-id="0a96f-111">The organizational level code defines the type or category of the organizational level, such a CEO  or CFO.</span></span> <span data-ttu-id="0a96f-112">Sie können mehrere Positionscodes haben.</span><span class="sxs-lookup"><span data-stu-id="0a96f-112">You can have several organizational level codes.</span></span> <span data-ttu-id="0a96f-113">Um die Position zu definieren, verwenden Sie das **Positionen**-Fenster.</span><span class="sxs-lookup"><span data-stu-id="0a96f-113">To define the organizational level, you use the **Organizational Levels** window.</span></span>

1. <span data-ttu-id="0a96f-114">Wählen Sie das Symbol ![Nach Seite oder Bericht suchen](media/ui-search/search_small.png "Nach Seite oder Bericht suchen") und geben **Positionen** ein. Wählen Sie dann den zugehörigen Link aus.</span><span class="sxs-lookup"><span data-stu-id="0a96f-114">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Organizational Levels**, and then choose the related link.</span></span>
2. <span data-ttu-id="0a96f-115">Wählen Sie die Aktion **Neu** aus, und geben Sie einen Code und eine Beschreibung ein.</span><span class="sxs-lookup"><span data-stu-id="0a96f-115">Choose the **New** action, and fill in a code and description.</span></span> <span data-ttu-id="0a96f-116">Der Code kann maximal 11 Zeichen, sowohl Ziffern als auch Buchstaben, umfassen.</span><span class="sxs-lookup"><span data-stu-id="0a96f-116">The code can be a maximum of 11 characters, and can be any combination of numbers and letters.</span></span>

## <a name="to-assign-organizational-levels-to-a-contact-person"></a><span data-ttu-id="0a96f-117">Um Organisationsstufen einer Kontaktperson zuzuweisen</span><span class="sxs-lookup"><span data-stu-id="0a96f-117">To assign organizational levels to a contact person</span></span>
<span data-ttu-id="0a96f-118">Sie können Positionen nur zu Kontaktpersonen zuweisen, nicht zu Unternehmen.</span><span class="sxs-lookup"><span data-stu-id="0a96f-118">You can assign organizational levels to contact persons only, not contact companies.</span></span> <span data-ttu-id="0a96f-119">Sie können jedem Kontakt nur eine Position zuordnen.</span><span class="sxs-lookup"><span data-stu-id="0a96f-119">You can only assign one organizational level to each contact.</span></span>

1. <span data-ttu-id="0a96f-120">Öffnen Sie den Kontakt.</span><span class="sxs-lookup"><span data-stu-id="0a96f-120">Open the contact.</span></span>
2. <span data-ttu-id="0a96f-121">Wählen Sie im Feld **Positionen** den Code aus, den Sie zuordnen möchten.</span><span class="sxs-lookup"><span data-stu-id="0a96f-121">In the **Organizational Levels** field, select the code you want to assign.</span></span>

<span data-ttu-id="0a96f-122">Nachdem Sie Ihren Kontakten Positionen zugeordnet haben, können Sie diese Informationen verwenden, um Segmente zu erstellen.</span><span class="sxs-lookup"><span data-stu-id="0a96f-122">After you have assigned organizational levels to your contacts, you can use this information to create segments.</span></span>

<span data-ttu-id="0a96f-123">Sobald Sie Ihren Kontakten Verantwortlichkeiten zugeordnet haben, können Sie diese Informationen verwenden, um Kontakte für Ihre Segmente auszuwählen.</span><span class="sxs-lookup"><span data-stu-id="0a96f-123">After you have assigned job responsibilities to your contacts, you can use this information to select contacts for your segments.</span></span> <span data-ttu-id="0a96f-124">Weitere Informationen finden Sie unter [Hinzufügen von Kontakten zu Segmenten](marketing-add-contact-segment.md).</span><span class="sxs-lookup"><span data-stu-id="0a96f-124">For more information, see [Add Contacts to Segments](marketing-add-contact-segment.md).</span></span>

## <a name="see-also"></a><span data-ttu-id="0a96f-125">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="0a96f-125">See Also</span></span>
[<span data-ttu-id="0a96f-126">Kontaktunternehmenerstellen</span><span class="sxs-lookup"><span data-stu-id="0a96f-126">Creating Contact Companies</span></span>](marketing-create-contact-companies.md)  
[<span data-ttu-id="0a96f-127">Kontaktpersonen erstellen</span><span class="sxs-lookup"><span data-stu-id="0a96f-127">Creating Contact Persons</span></span>](marketing-create-contact-persons.md)  
<span data-ttu-id="0a96f-128">[Arbeiten mit [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="0a96f-128">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>  
