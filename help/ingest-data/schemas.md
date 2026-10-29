---
title: Schemata
description: Erfahren Sie, wie Sie die Schemata verwalten, die zur Aufnahme von Daten in Marketing Campaign Analytics erforderlich sind.
feature: Schemas
exl-id: 08289581-5af9-4422-b049-8c24105e2a8e
autotag-review: '2026-05-01T08:56:54.552Z'
TQID: 'https://experienceleague.adobe.com/GS91VDl1bmpHRPKVZTg6j-94nikFXXFHWLhoMoDWaw4'
product_v2:
  - id: b88c80e3-31df-4609-989d-d4dac0e6d973
    internal-label: Marketing Campaign Analytics
feature_v2:
  - id: a567f0f7-0057-4079-8ded-5b24cc25af15
    internal-label: Harmonized data
  - id: e0abf868-dae2-4c1c-83e9-b21799232845
    internal-label: Datasets
  - id: fbd94e4b-f9b8-42a4-8df5-3f917aabae24
    internal-label: Schemas
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
    internal-label: Admin
source-git-commit: 9d6bd798e97d36d49b7753dc9574b102efb3d6bf
workflow-type: tm+mt
source-wordcount: '618'
ht-degree: 7%
---
# Schemata

{{mm-mca-rebranding}}

So verwalten Sie Schemata, indem Sie die Daten unterstützen, die Sie in Experience Platform aufnehmen und in Marketing Campaign Analytics verwenden möchten:

1. Wechseln Sie zur Marketing Campaign Analytics-Benutzeroberfläche.

1. Wählen Sie ![Schemata](/help/assets/icons/Schemas.svg) **[!UICONTROL Schemas]** unter **[!UICONTROL SETUP]** aus.

Weitere Informationen dazu finden [ in der Übersicht ](https://experienceleague.adobe.com/docs/experience-platform/xdm/ui/overview.html?lang=en) Schemas-Benutzeroberfläche .

## Aggregierte oder zusammenfassende Daten

Es wird dringend empfohlen, die Klasse XDM Summary Metrics als Grundlage für das Schema zu verwenden, das allen Aggregat- oder Zusammenfassungsdaten zugrunde liegt, die Sie in Experience Platform aufnehmen und in Marketing Campaign Analytics verwenden möchten.

Verwenden Sie die Klasse XDM Summary Metrics für:

- Ummauerte Gartendaten, z. B. Daten von Facebook oder YouTube.

- Daten externer Faktoren, wie Daten von SPX (S&amp;P 500 Aktienpreisindizes), Wetterdaten,

- Daten zu internen Faktoren, z. B. Preisänderungen, Feiertagskalender.

>[!IMPORTANT]
>
>Die Schemadefinition muss mindestens ein numerisches Feld enthalten (mit Ganzzahl, Doppelt, Boolesch oder einem anderen numerischen Typ), um die erforderlichen Metriken für die aufgenommenen Daten zu unterstützen.

Ein Schema, das die **[!DNL XDM Summary Metrics]** Basisklasse verwendet, kann einfach sein, wie in der folgenden **[!DNL ExternalFactorSummarySchema]** dargestellt.

![Schema „Externe Faktoren](/help/assets/external-factors-schema.png)

Dieses einfache Schema kann verwendet werden, um Datensätze aufzunehmen, die Daten enthalten für z. B.:

- Wettbewerbsindexdaten

  | Zeitstempel | date_type | Faktor | value |
  |---|---|---|--:|
  | 28.11.2020 T00:00:00.000Z | Woche | Competitor_index | 289.8 |
  | 2020-12-05T00:00:00.000Z | Woche | Competitor_index | 291.2 |
  | 2020-12-12T00:00:00.000Z | Woche | Competitor_index | 280.07 |
  | ... | ... | ... | ... |

- Daten zu Feiertagen

  | Zeitstempel | date_type | Faktor | value |
  |---|---|---|--:|
  | 28.11.2020 T00:00:00.000Z | Woche | all_hosts_flag | 0.0 |
  | 2020-12-05T00:00:00.000Z | Woche | all_hosts_flag | 0.0 |
  | 2020-12-12T00:00:00.000Z | Woche | all_hosts_flag | 0.0 |
  | 2020-12-19T00:00:00.000Z | Woche | all_hosts_flag | 0.0 |
  | 26.12.2020:00:00.000Z | Woche | all_hosts_flag | 1.0 |
  | ... | ... | ... | ... |


Unten finden Sie ein umfassendes Beispiel für eine **[!DNL LumaPaidMarketingSchema]**, bei der die **[!DNL XDM Summary Metrics]** als Basisklasse verwendet wird. Das Schema verwendet dedizierte Feldergruppen (mit Farben kommentiert) für Metriken (**[!DNL AMMMetrics]**), Dimensionen (**[!DNL AMMDimensions]**) und andere kundenspezifische Informationen (**[!DNL CustomerSpecific]**).

![Zusammenfassungsschema](/help/assets/summary-schema.png)

Da die Profilaufnahme asynchron erfolgt, wird empfohlen, bei der Erfassung von Aggregat- oder Zusammenfassungsdaten aus externen Quellen die Feldergruppe Audit-Details des externen Source-Systems als Teil eines Schemas zu verwenden. Diese Feldergruppe definiert einen Satz von Audit-Eigenschaften für externe Quellen.

## Feldergruppe „Standardfelder“

Zur Vereinfachung unterstützt Experience Platform eine dedizierte Feldergruppe „Standardfaktorfelder“ für interne und externe Faktordaten, die häufig Teil von Zusammenfassungs-, internen oder externen Faktordaten sind. Diese Feldergruppe definiert die folgenden Felder:

| Anzeigename des Feldes | Feldname | Feldtyp | Datentyp | Erforderlich | Beschreibung |
|---|---|---|---|:-:|---|
| Faktorname | factorName | Dimension | Zeichenfolge | ![Häkchen](/help/assets/icons/Checkmark.svg) | Der Name des Faktors |
| Faktorwert | faktorValue | Metrik | Double | ![Häkchen](/help/assets/icons/Checkmark.svg) | Der Wert des Faktors |
| Faktortyp | factorType | Dimension | Zeichenfolge (enum) | | Der Typ des Faktors.<br/>Mögliche Werte sind: <ul><li>Intern (interner Faktor)</li><li>Extern (externer Faktor)</li></ul> |
| Werttyp | valueType | Dimension | Zeichenfolge (enum) | | Mögliche Werte sind:<ul><li>Ist (tatsächlicher Wert)</li><li>Prognostiziert (prognostizierter Wert)</li></ul>Wenn kein Wert vorhanden ist, wird der Standardwert Actual verwendet. |
| Granularität | Granularität | Dimension | Zeichenfolge (enum) | | Mögliche Werte sind:<ul><li>Täglich</li><li>Wöchentlich</li><li>Monatlich</li></ul> |

Ein Zusammenfassungs-, interner Faktor- oder externer Faktor-Datensatz kann auf Folgendem basieren:

- Ein Schema, **die Gruppe** Standardfelder“ verwendet. Dieser Datensatz wird beim Konfigurieren von Datensatzregeln als **[!UICONTROL Factors]** Datensatz angezeigt. Die harmonisierten Felder, die Sie als Teil der Datensatzregeln für den Datensatz definieren, stehen beim Erstellen eines Modells als Faktoren zur Verfügung.
- Ein Schema, das **Gruppe der**-Standardfelder verwendet. Dieser Datensatz wird beim Konfigurieren von Datensatzregeln als **[!UICONTROL Summary]** Datensatz angezeigt. Der Datensatz ist als Zusammenfassungsdaten konfiguriert und beeinflusst keine harmonisierten Daten.

## Unterstützte Datentypen

Derzeit unterstützt Marketing Campaign Analytics eine Untergruppe von Experience Platform-Datentypen nicht. Die folgenden grundlegenden Datentypen (Felder), die unter [Grundlagen der Schemakomposition](https://experienceleague.adobe.com/docs/experience-platform/xdm/schema/composition.html?lang=en#data-type) erwähnt werden, werden unterstützt:

- Zeichenfolge
- Ganzzahl
- Double
- Boolesch
- Lang
- Kurz
- Byte
- Datum
- Datum-Uhrzeit


>[!MORELIKETHIS]
>
>- [Schemata](schemas.md)
