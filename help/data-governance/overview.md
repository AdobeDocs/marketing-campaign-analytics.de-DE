---
title: Übersicht zur Data Governance
description: Erfahren Sie, wie Sie die Services und Tools von Experience Platform verwenden, mit denen Sie Ihre erfassten Erlebnisdaten steuern können. So halten Sie Ihre Geschäftspraktiken, rechtlichen Verpflichtungen und Ihren Entwicklungsprozess ein.
feature: Administration
exl-id: 87407c29-e158-48bf-bde9-b3c16a16107e
autotag-review: '2026-05-01T09:16:50.195Z'
TQID: 'https://experienceleague.adobe.com/4a-Y6-emQcZoHGcJwEttb4wcMyrxQvsbXRZ0SDpNhTs'
product_v2:
  - id: b88c80e3-31df-4609-989d-d4dac0e6d973
    internal-label: Marketing Campaign Analytics
feature_v2:
  - id: a567f0f7-0057-4079-8ded-5b24cc25af15
    internal-label: Harmonized data
  - id: e0abf868-dae2-4c1c-83e9-b21799232845
    internal-label: Datasets
  - id: f40f1683-8300-4054-aab8-77da06ad63ff
    internal-label: Models
  - id: f6633d1c-3d2d-4f48-95d4-4bbc9913db52
    internal-label: Data governance
  - id: fe2edbb1-46f9-4347-a27c-577cab3640cb
    internal-label: Administration
subfeature_v2:
  - id: bf7ac0fc-effb-4f0c-b93f-658412718d3c
    internal-label: Audits
  - id: fd80ec6b-9b9e-448a-a6d0-b0c9a15da6b8
    internal-label: Policies
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
    internal-label: Admin
topic_v2:
  - id: b4dd41a7-ccf8-4e9d-918e-acaab534a307
    internal-label: Data quality
  - id: c7d04a2c-412a-4c9d-9d7a-4456eaa5adeb
    internal-label: Governance
  - id: d095671a-1355-40aa-8b5f-06c33c68080b
    internal-label: Security
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
  - id: f4e6943a-c91a-4134-a2c7-f4f20cfff2f0
    internal-label: Privacy
source-git-commit: 9d6bd798e97d36d49b7753dc9574b102efb3d6bf
workflow-type: tm+mt
source-wordcount: '469'
ht-degree: 11%
---
# Übersicht zur Data Governance

{{mm-mca-rebranding}}

Die Integration zwischen Marketing Campaign Analytics und Experience Platform bietet Marketing Campaign Analytics die Möglichkeit, die internen Data Governance-Funktionen von Experience Platform zu nutzen. In diesem Abschnitt der Dokumentation werden die Besonderheiten der in Marketing Campaign Analytics verfügbaren Data Governance-Funktionen beschrieben.

Experience Platform Data Governance bietet Ihnen die Möglichkeit, Ihre Daten über den gesamten Journey, den Daten über Experience Platform durchlaufen, zu kontrollieren und zu erfassen. Diese Journey umfasst die Aufrechterhaltung der Datenqualität, der Datenherkunft, der Datenkatalogisierung und vieles mehr.

Datennutzungsbeschriftungen und -richtlinien, die für Datensätze erstellt werden, die von der Experience Platform-Oberfläche in der Marketing Campaign Analytics genutzt werden, sofern zutreffend. Beispielsweise stoppen oder warnen diese Kennzeichnungen Benutzende, wenn sie Datensätze löschen, die Teil einer Datensatzregel in den harmonisierten Daten sind. Oder blenden Sie Schemafelder aus, die beim Erstellen einer Datensatzregel für Benutzer eingeschränkt sind.

Die Data Governance-Integration ermöglicht ein effizienteres Compliance-Management. Datenverantwortliche in Ihrem Unternehmen können Richtlinien festlegen, um die Nutzung zu beschränken. So können Sie Daten verwenden, die den von Datenverantwortlichen definierten Richtlinien entsprechen. Weitere Informationen finden Sie in der Dokumentation zu [Labels und Richtlinien](https://experienceleague.adobe.com/en/docs/analytics-platform/using/cja-dataviews/data-governance).

Die folgenden Data Governance-Funktionen sind verfügbar:

| Funktion | Details |
|---|---|
| Zugriffssteuerungen | Es werden die rollenbasierte Zugriffssteuerung und die attributbasierte Zugriffssteuerung (auf Feldebene) unterstützt. Weitere Informationen finden [ unter ](access-controls.md). |
| Auditprotokolle | Wenn Benutzende bestimmte Marketing Campaign Analytics-Kategorien erstellen, aktualisieren oder löschen, zeichnet die Experience Platform-Überwachungsfunktion die Aktivität in den Administratorprotokollen auf. Weitere [ finden Sie ](audit-logs.md) Auditprotokolle . |
| Richtlinien | Im Rahmen des harmonisierten Daten-Workflows werden von Experience Platform definierte Richtlinien durchgesetzt. Jeder Verstoß gegen Datennutzungskennzeichnungen wird gemeldet und dem Benutzer angezeigt. Weitere Informationen finden [ unter ](policies.md). |
| Verschlüsselung | Alle Datensätze, die für die Eingabe und Ausgabe von Modellen verwendet werden, entsprechen den Experience Platform-Richtlinien. Die Experience Platform-Datenverschlüsselung gilt für Daten im Ruhezustand und während der Übertragung. |
| Datenhygiene | Alle Datensätze, die für Eingabe- und Nicht-Modelle verwendet werden, entsprechen den Experience Platform-Richtlinien. Experience Platform bietet eine Reihe von Tools zur Verwaltung des Lebenszyklus von Kundendaten, einschließlich der Unterstützung verschiedener Arten von Datenablauf. Wenn Sie einen Quelldatensatz aus Experience Platform löschen, der als Teil Ihrer harmonisierten Daten verwendet wird, werden Sie benachrichtigt. Weitere Informationen [ Sie unter ](/help/harmonize-data/dataset-rules.md)Datensatzregeln“. |
| Kundenseitig verwaltete Schlüssel | Wenn Sie Marketing Campaign Analytics mit dem Privacy Security Shield-Add-on lizenziert haben, können Sie die Funktion für kundenseitig verwaltete Schlüssel verwenden, um Azure Key Vault zu nutzen und Ihre eigenen Schlüssel über APIs zu übertragen. Sie verfügen über eine vollständige Verwaltung von Daten, die innerhalb von Modellen in Marketing Campaign Analytics verarbeitet werden. |
