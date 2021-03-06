---
title: Synchronisierung und Datenintegration | Microsoft Docs
description: Bei der Synchronisation werden Daten zwischen Common Data Service-Entitäten und Business Centra-Datensätzen kopiert und die Daten in beiden Systemen auf dem neuesten Stand gehalten.
author: bholtorf
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: sales, crm, integration, sync, synchronize
ms.date: 04/01/2020
ms.author: bholtorf
ms.openlocfilehash: 01629cb7e881de1c679d8c6925eaacc3a5639597
ms.sourcegitcommit: d67328e1992c9a754b14c7267ab11312c80c38dd
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 04/01/2020
ms.locfileid: "3196471"
---
# <a name="synchronizing-data-in-business-central-with-common-data-service"></a>Synchronisieren von Daten in Business Central mit Common Data Service
Wenn Sie [!INCLUDE[d365fin](includes/cds_long_md.md)] in [!INCLUDE[d365fin](includes/d365fin_md.md)] integrieren, können Sie entscheiden, ob die Daten der ausgewählten Felder von [!INCLUDE[d365fin](includes/d365fin_md.md)]-Datensätzen (wie Debitoren, Kontakten und Vertriebsmitarbeitern) mit entsprechenden Datensätzen in [!INCLUDE[d365fin](includes/cds_long_md.md)] synchronisieren (beispielsweise Konten, Kontakte und Benutzer). Je nach Art des Datensatzes können Sie Daten von [!INCLUDE[d365fin](includes/cds_long_md.md)] nach [!INCLUDE[d365fin](includes/d365fin_md.md)] synchronisieren oder umgekehrt. Weitere Informationen finden Sie unter [Integrieren in Dynamics 365 Sales](admin-prepare-dynamics-365-for-sales-for-integration.md).  

Bei der Synchronisierung werden die folgenden Elemente einbezogen:

* Integrationstabellenzuordnungen
* Integrationsfeldzuordnungen
* Synchronisierungsregeln
* Gekoppelte Datensätze

Wenn die Synchronisierung eingerichtet ist, können Sie die [!INCLUDE[d365fin](includes/d365fin_md.md)]-Datensätze mit [!INCLUDE[d365fin](includes/cds_long_md.md)]-Datensätzen koppeln, um ihre Daten zu synchronisieren. Sie können eine Synchronisierung manuell oder nach Plan starten. Die folgende Tabelle zeigt eine Übersicht über die Methoden der Synchronisierung von Datensätzen.  

|  Typ  |  Art  |  Siehe  |  
|--------|----------|-------|  
|Manuelle Synchronisierung|Synchronisieren Sie auf Basis von Datensätzen.<br /><br /> Sie können, beispielsweise als Debitor, einzelne Datensätze in [!INCLUDE[d365fin](includes/d365fin_md.md)] mit einem entsprechenden [!INCLUDE[d365fin](includes/cds_long_md.md)]-Datensatz synchronisieren, beispielsweise einem Konto. So arbeiten Benutzer normalerweise mit [!INCLUDE[d365fin](includes/cds_long_md.md)]-Daten in [!INCLUDE[d365fin](includes/d365fin_md.md)].|[Datensätze manuell koppeln und synchronisieren](admin-manual-synchronization-of-table-mappings.md#synchronize-individual-table-mappings)|  
|  |Synchronisieren Sie auf Basis einer Tabellenzuordnung.<br /><br /> Sie können alle Datensätze in einer [!INCLUDE[d365fin](includes/d365fin_md.md)]-Tabelle mit einer [!INCLUDE[d365fin](includes/cds_long_md.md)]-Einheit synchronisieren.|[Synchronisieren einzelner Tabellenzuordnungen](admin-manual-synchronization-of-table-mappings.md#synchronize-individual-table-mappings)|  
||Synchronisieren Sie alle geänderten Datensätze für alle Tabellenzuordnungen.<br /><br /> Sie können alle Datensätze synchronisieren, die in den [!INCLUDE[d365fin](includes/d365fin_md.md)]-Tabellen seit der letzten Synchronisierung geändert wurden.|[Synchronisierung aller geänderten Datensätze](admin-manual-synchronization-of-table-mappings.md#synchronizing-all-modified-records)|
||Vollständige Synchronisierung aller Daten für alle Tabellenzuordnungen.<br /><br /> Sie können alle Daten in den [!INCLUDE[d365fin](includes/d365fin_md.md)]-Tabellen und die [!INCLUDE[d365fin](includes/cds_long_md.md)]-Einheiten, die zugeordnet werden, synchronisieren, und neue Datensätze in der Ziellösung für ungekoppelte Datensätze in der Quelllösung erstellen.<br /><br /> Bei der vollständigen Synchronisierung werden alle Daten synchronisiert und die Kopplung ignoriert. Normalerweise führen Sie eine vollständige Synchronisierung durch, wenn Sie die Integration einrichten und nur eine der Lösungen enthält Daten. Eine vollständige Synchronisierung kann auch in einer Demonstrationsumgebung hilfreich sein.|[Ausführen einer vollständigen Synchronisierung](admin-manual-synchronization-of-table-mappings.md#run-a-full-synchronization)|  
|Geplante Synchronisierung|Synchronisieren Sie alle Änderungen an Daten für alle Tabellenzuordnungen.<br /><br /> Sie können [!INCLUDE[d365fin](includes/d365fin_md.md)] mit [!INCLUDE[d365fin](includes/cds_long_md.md)] in geplanten Intervallen synchronisieren, indem Sie Projekte in der Projektwarteschlange einrichten.|[Planen einer Synchronisierung](admin-scheduled-synchronization-using-the-synchronization-job-queue-entries.md)|  

## <a name="standard-entity-mapping-for-synchronization"></a>Standard-Entitätszuordnung für die Synchronisierung
Entitäten in [!INCLUDE[d365fin](includes/cds_long_md.md)] wie beispielsweise Konten, werden mit äquivalenten Arten von Entitäten in [!INCLUDE[d365fin](includes/d365fin_md.md)] wie beispielsweise Debitoren integriert. Um mit [!INCLUDE[d365fin](includes/cds_long_md.md)]-Daten zu arbeiten, richten Sie Verknüpfungen, auch Kopplungen genannt, zwischen Einheiten in [!INCLUDE[d365fin](includes/cds_long_md.md)] und [!INCLUDE[d365fin](includes/d365fin_md.md)] ein.

Die folgende Tabelle zeigt die standardmäßige Zuordnung zwischen Einheiten in [!INCLUDE[d365fin](includes/d365fin_md.md)] und [!INCLUDE[d365fin](includes/d365fin_md.md)], die [!INCLUDE[d365fin](includes/cds_long_md.md)] bietet.

|[!INCLUDE[d365fin](includes/d365fin_md.md)]|[!INCLUDE[d365fin](includes/cds_long_md.md)]|Synchronisierungsrichtung|Standardfilter|
|-------------------------------------------|-----|-------------------------|--------------|
|Verkäufer/Einkäufer|Benutzer|[!INCLUDE[d365fin](includes/cds_long_md.md)] -> [!INCLUDE[d365fin](includes/d365fin_md.md)]|Vertriebskontaktfilter: **Status** ist **Nein**, **Benutzer lizenziert** **Ja** ist, Integrationsbenutzer Modus ist **Nein**|
|Debitor|Konto|[!INCLUDE[d365fin](includes/d365fin_md.md)] -> [!INCLUDE[crm_md](includes/crm_md.md)] und [!INCLUDE[crm_md](includes/crm_md.md)] -> [!INCLUDE[d365fin](includes/d365fin_md.md)]|Sales-Kontenfilter: **Verhältnisart** ist **Debitor** und **Status** ist **Aktiv**.|
|Kreditor|Konto|[!INCLUDE[d365fin](includes/d365fin_md.md)] -> [!INCLUDE[crm_md](includes/crm_md.md)] und [!INCLUDE[crm_md](includes/crm_md.md)] -> [!INCLUDE[d365fin](includes/d365fin_md.md)]|Filter für Vertriebskonten: **Beziehungstyp** ist **Kreditor** und **Status** ist **Aktiv**.|
|Kontakt|Kontakt|[!INCLUDE[d365fin](includes/d365fin_md.md)] -> [!INCLUDE[crm_md](includes/crm_md.md)] und [!INCLUDE[crm_md](includes/crm_md.md)] -> [!INCLUDE[d365fin](includes/d365fin_md.md)]|[!INCLUDE[d365fin](includes/d365fin_md.md)] Kontaktfilter: **Type** ist **Person** und der Kontakt wird einem Unternehmen zugewiesen. Sales Kontaktfilter: Kontakt wird einem Unternehmen zugeordnet und die übergeordnete Debitorenart ist **Konto**.|
|Währung|Transaktionswährung|[!INCLUDE[d365fin](includes/d365fin_md.md)] -> [!INCLUDE[crm_md](includes/crm_md.md)]| |


### <a name="tip-for-admins-viewing-entity-mappings"></a>Tipp für Administratoren: Aufrufen von Einheitenzuordnungen
Sie können die Zuordnung zwischen den Einheiten in [!INCLUDE[d365fin](includes/cds_long_md.md)] und den Tabellen in [!INCLUDE[d365fin](includes/d365fin_md.md)] auf der Seite **Integrationstabellenzuordnungen** aufrufen, auf der Sie auch Filter anwenden können. Sie legen die Zuordnung zwischen den Feldern in [!INCLUDE[d365fin](includes/d365fin_md.md)]-Tabellen und den Feldern in [!INCLUDE[d365fin](includes/cds_long_md.md)]-Einheiten auf der Seite **Integrationsfeldzuordnung** fest, auf der Sie zusätzliche Zuordnungslogiken hinzufügen können. Dies kann beispielsweise hilfreich sein, wenn Sie Fehler bei der Synchronisierung beheben müssen.

## <a name="see-also"></a>Siehe auch  
[Datensätze manuell koppeln und synchronisieren](admin-how-to-couple-and-synchronize-records-manually.md)   
[Planen einer Synchronisierung](admin-scheduled-synchronization-using-the-synchronization-job-queue-entries.md)   
[Integration mit Dynamics 365 Sales](admin-prepare-dynamics-365-for-sales-for-integration.md)
