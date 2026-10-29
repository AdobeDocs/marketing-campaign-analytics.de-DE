---
title: Auditprotokolle
description: Erfahren Sie, wie Sie von Marketing Campaign Analytics aus auf Auditprotokolle zugreifen können.
feature: Administration
exl-id: aa65aac5-bea4-43ff-b0d0-9e8a6a97d3ca
autotag-review: '2026-05-01T09:16:13.122Z'
TQID: 'https://experienceleague.adobe.com/ZH89ZDOEMDwbvU5QnPtpkDft0U121-JDrhgEBPDuV3Q'
product_v2:
  - id: b88c80e3-31df-4609-989d-d4dac0e6d973
    internal-label: Marketing Campaign Analytics
feature_v2:
  - id: f6633d1c-3d2d-4f48-95d4-4bbc9913db52
    internal-label: Data governance
  - id: fe2edbb1-46f9-4347-a27c-577cab3640cb
    internal-label: Administration
subfeature_v2:
  - id: bf7ac0fc-effb-4f0c-b93f-658412718d3c
    internal-label: Audits
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
    internal-label: Admin
topic_v2:
  - id: a004cc84-67b9-4a33-a3a7-8ec7273ef4dc
    internal-label: Metadata
  - id: c1579802-ddd4-4214-8a91-97b2066abe11
    internal-label: Troubleshooting
  - id: c7d04a2c-412a-4c9d-9d7a-4456eaa5adeb
    internal-label: Governance
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
  - id: f4e6943a-c91a-4134-a2c7-f4f20cfff2f0
    internal-label: Privacy
source-git-commit: 9d6bd798e97d36d49b7753dc9574b102efb3d6bf
workflow-type: tm+mt
source-wordcount: '519'
ht-degree: 12%
---
# Auditprotokolle

{{mm-mca-rebranding}}

Um die Transparenz und Sichtbarkeit der im System durchgeführten Aktivitäten zu erhöhen, werden Benutzeraktivitäten innerhalb des Marketing Campaign Analytics-Workflows in Experience Platform-Auditprotokollen erfasst, um benutzergesteuerte Änderungen an Marketing Campaign Analytics-Kategorien zu verstehen. Diese Protokolle bilden einen Audit-Trail, der Ihnen bei der Fehlerbehebung und Ihrem Unternehmen helfen kann, die Richtlinien zur Unternehmensdatenverwaltung und die gesetzlichen Anforderungen effektiv zu erfüllen.

<!-- 
DO WE HAVE TO ADD THIS
If you are subject to the Health Insurance Portability and Accountability Act (HIPAA) and create, receive, maintain, or transmit permitted sensitive personal data through Marketing Campaign Analytics, you are responsible for executing a BAA with Adobe and licensing Healthcare Shield.
-->

Ein Auditprotokoll informiert darüber, wer welche Aktion wann ausgeführt hat. Jede in einem Protokoll aufgezeichnete Aktion enthält Metadaten, die den Aktionstyp, das Datum und die Uhrzeit, die E-Mail-ID der oder des Benutzenden, die oder der die Aktion durchgeführt hat, und weitere für den Aktionstyp relevante Attribute angeben. Es verfolgt die von Benutzenden in Marketing Campaign Analytics durchgeführten Aktionen zum Erstellen, Aktualisieren und Löschen.

So überprüfen Sie das Administratorprotokoll in der Benutzeroberfläche von Marketing Campaign Analytics:

1. Wählen Sie ![Aufgabenliste](/help/assets/icons/TaskList.svg) **[!UICONTROL Audits]** aus **[!UICONTROL PRIVACY]** aus.

1. In **[!UICONTROL Audits]** finden Sie die **[!UICONTROL Activity log]**. Das Aktivitätsprotokoll zeigt Einträge für die folgenden Marketing Campaign Analytics-Kategorien, -Aktionen und -Status an.

   | Kategorie | Aktion | Status |
   |---|---|---|
   | Marketing Campaign Analytics-Datensatzregel | Erstellen | Zulassen oder Ablehnen |
   | Marketing Campaign Analytics-Datensatzregel | Update | Zulassen oder Ablehnen |
   | Marketing Campaign Analytics-Datensatzregel | Löschen | Zulassen oder Ablehnen |
   | Marketing Campaign Analytics-Feld | Erstellen | Zulassen oder Ablehnen |
   | Marketing Campaign Analytics-Feld | Update | Zulassen oder Ablehnen |
   | Marketing Campaign Analytics-Feld | Löschen | Zulassen oder Ablehnen |
   | Marketing Campaign Analytics Marketing Touchpoint | Erstellen | Zulassen oder Ablehnen |
   | Marketing Campaign Analytics Marketing Touchpoint | Update | Zulassen oder Ablehnen |
   | Marketing Campaign Analytics Marketing Touchpoint | Löschen | Zulassen oder Ablehnen |
   | Marketing Campaign Analytics-Konversion | Erstellen | Zulassen oder Ablehnen |
   | Marketing Campaign Analytics-Konversion | Update | Zulassen oder Ablehnen |
   | Marketing Campaign Analytics-Konversion | Löschen | Zulassen oder Ablehnen |
   | Marketing Campaign Analytics-Modell | Erstellen | Zulassen oder Ablehnen |
   | Marketing Campaign Analytics-Modell | Update | Zulassen oder Ablehnen |
   | Marketing Campaign Analytics-Modell | Löschen | Zulassen oder Ablehnen |
   | Marketing Campaign Analytics-Modell | neu bewerten | Zulassen oder Ablehnen |
   | Marketing Campaign Analytics-Modell | Klonen | Zulassen oder Ablehnen |
   | Marketing Campaign Analytics-Modell | Trainieren/Umschulen | Zulassen oder Ablehnen |
   | Marketing Campaign Analytics-Modell | Herunterladen/Speichern von Metadaten | Zulassen oder Ablehnen |
   | Marketing Campaign Analytics-Plan | Erstellen | Zulassen oder Ablehnen |
   | Marketing Campaign Analytics-Plan | Update | Zulassen oder Ablehnen |
   | Marketing Campaign Analytics-Plan | Zugehöriges Modell ändern | Zulassen oder Ablehnen |
   | Marketing Campaign Analytics-Datenharmonisierung | Trigger Sync | Zulassen oder Ablehnen |


1. Wählen Sie einen Eintrag im Aktivitätsprotokoll aus, um ein Bedienfeld mit weiteren Details zu öffnen.

   ![Marketing Campaign Analytics-Audit](/help/assets/mix-modeler-audit.png)

1. Um nach **[!UICONTROL Category]**, **[!UICONTROL Action]**, **[!UICONTROL Request ID]**, **[!UICONTROL User]**, **[!UICONTROL Status]** oder **[!UICONTROL Date]** Bereich zu filtern, wählen Sie ![Filter](/help/assets/icons/Filter.svg).

1. Um die im Aktivitätsprotokoll angezeigten Spalten zu ändern, wählen Sie ![Spalten](/help/assets/icons/ColumnSetting.svg) und im Dialogfeld &quot;**[!UICONTROL Customize table]**&quot; die anzuzeigenden Spalten aus. Wählen Sie **[!UICONTROL Apply]** aus, um die Auswahl anzuwenden, **[!UICONTROL Cancel]** um sie aufzuheben.

1. Um das Administratorprotokoll herunterzuladen, wählen Sie ![Herunterladen](/help/assets/icons/Download.svg) **[!UICONTROL Download log]**. Wählen Sie im Dialogfeld **[!UICONTROL Download log]** entweder **[!UICONTROL CSV]** oder **[!UICONTROL JSON]** als Format aus und klicken Sie auf **[!UICONTROL Download]**.

## Zugriff auf Auditprotokolle

Wenn die Funktion für Ihr Unternehmen aktiviert ist, werden bei Aktivitäten automatisch Auditprotokolle erfasst. Die Auditprotokollerfassung muss nicht manuell aktiviert werden.

Um Auditprotokolle anzeigen und exportieren zu können, benötigen Sie die Zugriffsberechtigung Zugriff auf Auditprotokolle . Informationen zum Verwalten individueller Berechtigungen für Marketing Campaign Analytics-Funktionen finden Sie in der [Dokumentation zur Zugriffssteuerung](https://experienceleague.adobe.com/de/docs/experience-platform/access-control/home).
