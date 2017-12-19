---
title: "Möglichkeit für die Problembehebung oder Umgehung von Problemen | Microsoft Docs"
description: Erfahren Sie, wie Sie um jegliche Probleme im Accountant Hub for Dynamics 365 umgehen.
author: edupont04
ms.service: dynamics365-accountant
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: accountant, accounting, troubleshoot
ms.date: 10/23/2017
ms.author: edupont
ms.translationtype: HT
ms.sourcegitcommit: ba26b354d235981bd7291f9ac6402779f554ac7a
ms.openlocfilehash: a9753b00b47fc4d74583482b2da92aae5e2f8a74
ms.contentlocale: de-de
ms.lasthandoff: 11/10/2017

---
# <a name="troubleshooting-included365acclongincludesd365acclongmdmd"></a><span data-ttu-id="b2812-103">Problembehebung [!INCLUDE[d365acc_long](includes/d365acc_long_md.md)]</span><span class="sxs-lookup"><span data-stu-id="b2812-103">Troubleshooting [!INCLUDE[d365acc_long](includes/d365acc_long_md.md)]</span></span>
[!INCLUDE[d365fin_early_release](includes/d365fin_early_release.md.md)]

<span data-ttu-id="b2812-104">Die Anmeldung für [!INCLUDE[d365acc](includes/d365acc_md.md)] ist einfach und kann sehr schnell vorgenommen werden.</span><span class="sxs-lookup"><span data-stu-id="b2812-104">Signing up for [!INCLUDE[d365acc](includes/d365acc_md.md)] is easy and can be done very quickly.</span></span> <span data-ttu-id="b2812-105">Das Hinzufügen von Kundens zum Dashboard ist auch einfach, aber in diesem Artikel werden Probleme behandelt, die dabei auftreten können.</span><span class="sxs-lookup"><span data-stu-id="b2812-105">Adding clients to the dashboard is also easy, but this article addresses issues that you may have on the way.</span></span>

## <a name="what-email-address-can-i-use-with-included365accincludesd365accmdmd"></a><span data-ttu-id="b2812-106">Welche E-Mail-Adresse kann ich mit [!INCLUDE[d365acc](includes/d365acc_md.md)]?</span><span class="sxs-lookup"><span data-stu-id="b2812-106">What email address can I use with [!INCLUDE[d365acc](includes/d365acc_md.md)]?</span></span>
[!INCLUDE[d365acc](includes/d365acc_md.md)]<span data-ttu-id="b2812-107"> erfordert eine Arbeits- oder Schul-E-Mail-Adresse, um sich anzumelden.</span><span class="sxs-lookup"><span data-stu-id="b2812-107"> requires that you use a work or school email address to sign up.</span></span> [!INCLUDE[d365acc](includes/d365acc_md.md)]<span data-ttu-id="b2812-108"> unterstützt keine E-Mail-Adressen, die von E-Mail-Diensten für Endverbraucher oder Telekommunikationsanbietern bereitgestellt werden.</span><span class="sxs-lookup"><span data-stu-id="b2812-108"> does not support email addresses provided by consumer email services or telecommunication providers.</span></span> <span data-ttu-id="b2812-109">Dieses schließt outlook.com, hotmail.com, gmail.com und andere ein.</span><span class="sxs-lookup"><span data-stu-id="b2812-109">This includes outlook.com, hotmail.com, gmail.com, and others.</span></span>  

<span data-ttu-id="b2812-110">Wenn Sie versuchen, sich mit einer persönlichen E-Mail-Adresse anzumelden, erhalten Sie eine Meldung die angibt, eine Arbeits- oder Schul-E-mail-Adresse zu verwenden.</span><span class="sxs-lookup"><span data-stu-id="b2812-110">If you try to sign up with a personal email address, you will get a message indicating to use a work or school email address.</span></span>  

## <a name="why-cant-i-connect-to-my-clients-data"></a><span data-ttu-id="b2812-111">Warum nicht kann ich keine Verbindung zu den Daten meines Kundens herstellen?</span><span class="sxs-lookup"><span data-stu-id="b2812-111">Why can't I connect to my client's data?</span></span>
<span data-ttu-id="b2812-112">Es kann mehrere Gründe geben, unter anderem die Folgenden:</span><span class="sxs-lookup"><span data-stu-id="b2812-112">There can be a couple of reasons, including the following:</span></span>

- <span data-ttu-id="b2812-113">Die URL im Feld **Kunden URL** ist ungültig</span><span class="sxs-lookup"><span data-stu-id="b2812-113">The URL in the **Client URL** field is not valid</span></span>  

  <span data-ttu-id="b2812-114">Wechseln zu **Manage Kundens**, öffnen Sie den Kunden, zu dem Sie keine Verbindung herstellen können, und wählen Sie dann **Test Kunden URL** aus.</span><span class="sxs-lookup"><span data-stu-id="b2812-114">Go to **Manage Clients**, open the client that you cannot connect to, and then choose **Test Client URL**.</span></span>  
- <span data-ttu-id="b2812-115">Das Unternehmen des Kundens ist derzeit offline, beispielsweise bei einem Upgrade</span><span class="sxs-lookup"><span data-stu-id="b2812-115">The client's company is currently offline, for example if it being upgraded</span></span>

  <span data-ttu-id="b2812-116">Wählen Sie in Ihrem Dashboard das Menüelement **Werkzeuge** aus, und wählen Sie dann **Fehler prüfen**.</span><span class="sxs-lookup"><span data-stu-id="b2812-116">In your dashboard, choose the **Tools** menu item, and then choose **Check Errors**.</span></span> <span data-ttu-id="b2812-117">Dadurch wird eine Liste mit technischen Details geöffnet, daher sollten Sie sich an Ihren Administrator wenden, wenn Sie Fehler finden.</span><span class="sxs-lookup"><span data-stu-id="b2812-117">This opens a list with technical details, so you might want to contact your administrator if you're seeing errors.</span></span> <span data-ttu-id="b2812-118">Zum Beispiel weist die Fehlermeldung "Der Server hat die Anmeldeinformationen des Kundens abgelehnt" darauf hin, dass Sie keinen Zugriff haben.</span><span class="sxs-lookup"><span data-stu-id="b2812-118">For example, the error message "The server has rejected the client credentials" suggests that you do not have access.</span></span>  
- <span data-ttu-id="b2812-119">Sie haben keine E-Mail von Ihrem Kunden erhalten, in der sie zu [!INCLUDE[d365fin](includes/d365fin_md.md)] eingeladen werden, oder Sie haben den Link in einer E-Mail nicht geöffnet, oder Sie haben die Einladung nicht angenommen</span><span class="sxs-lookup"><span data-stu-id="b2812-119">You have not received an email from your client that invites them to their [!INCLUDE[d365fin](includes/d365fin_md.md)], or you did not open the link in the email, or you did not accept the invitation</span></span>

  <span data-ttu-id="b2812-120">Sie müssen den Link in der Einladung öffnen und die Schritte akzeptieren, mit denen Sie zum [!INCLUDE[d365fin](includes/d365fin_md.md)] Ihres Kundens hinzugefügt werden.</span><span class="sxs-lookup"><span data-stu-id="b2812-120">You must open the link in the invitation and accept the steps that adds you to your client's [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span> <span data-ttu-id="b2812-121">Bis dahin haben Sie keinen Zugriff auf deren Daten.</span><span class="sxs-lookup"><span data-stu-id="b2812-121">Until then, you do not have access to their data.</span></span>  
- <span data-ttu-id="b2812-122">Sie haben keinen Zugriff auf alle Unternehmen in [!INCLUDE[d365fin](includes/d365fin_md.md)] Ihres Kundens</span><span class="sxs-lookup"><span data-stu-id="b2812-122">You do not have access to all companies in your client's [!INCLUDE[d365fin](includes/d365fin_md.md)]</span></span>

  <span data-ttu-id="b2812-123">Ihr Kunden kann über mehrere Konzernmandanten oder Mandanten in [!INCLUDE[d365fin](includes/d365fin_md.md)] verfügen und Ihre Einladung berücksichtigt nicht immer alle Unternehmen.</span><span class="sxs-lookup"><span data-stu-id="b2812-123">Your client can have multiple business units or companies in [!INCLUDE[d365fin](includes/d365fin_md.md)], and your invitation does not always include all companies.</span></span> <span data-ttu-id="b2812-124">Arbeiten Sie mit Ihrem Kunden, um sicherzustellen, dass Sie Zugriff auf die Unternehmen haben, in denen der Kunden Sie arbeiten lassen möchte.</span><span class="sxs-lookup"><span data-stu-id="b2812-124">Work with your client to make sure that you have access to the companies that the client wants you to work in.</span></span>  

## <a name="why-doesnt-the-data-refresh-in-my-dashboard"></a><span data-ttu-id="b2812-125">Warum werden die Daten in meinem Dashboard nicht aktualisiert?</span><span class="sxs-lookup"><span data-stu-id="b2812-125">Why doesn't the data refresh in my dashboard?</span></span>
<span data-ttu-id="b2812-126">Wenn Sie einen Kunden hinzufügen oder eine Aktualisierung der Daten anfordern, ruft [!INCLUDE[d365acc](includes/d365acc_md.md)] die Daten ab.</span><span class="sxs-lookup"><span data-stu-id="b2812-126">When you add a client or request a refresh of the data, [!INCLUDE[d365acc](includes/d365acc_md.md)] fetches the data.</span></span> <span data-ttu-id="b2812-127">Sie müssen das Fenster allerdings selbst aktualisieren, z. B. durch Auswählen der Aktion "Alle Unternehmen neu laden", das Browser-Fenster aktualisieren, vom Dashboard fort und wieder dorthin zurück navigieren oder etwas Ähnliches durchführen.</span><span class="sxs-lookup"><span data-stu-id="b2812-127">But you must refresh the window yourself, such as choosing the "Redisplay all companies" action, refresh the browser window, navigate away from the dashboard and then back again, or similar.</span></span> <span data-ttu-id="b2812-128">Dieses ist ein bekanntes Problem, an dessen Verbesserung in einem späteren Update wir arbeiten.</span><span class="sxs-lookup"><span data-stu-id="b2812-128">This is a known issue that we are working on improving in a later update.</span></span>  

## <a name="see-also"></a><span data-ttu-id="b2812-129">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="b2812-129">See Also</span></span>
<span data-ttu-id="b2812-130">[Erste Schritte mit [!INCLUDE[d365acc](includes/d365acc_md.md)]](get-started.md)</span><span class="sxs-lookup"><span data-stu-id="b2812-130">[Get Started with [!INCLUDE[d365acc](includes/d365acc_md.md)]](get-started.md)</span></span>  
<span data-ttu-id="b2812-131">[Fügen Sie Ihren Dashboard in [!INCLUDE[d365acc](includes/d365acc_md.md)]](add-client.md) Kunden hinzu</span><span class="sxs-lookup"><span data-stu-id="b2812-131">[Add Clients to Your Dashboard in [!INCLUDE[d365acc](includes/d365acc_md.md)]](add-client.md)</span></span>  
