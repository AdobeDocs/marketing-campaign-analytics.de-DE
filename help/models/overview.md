---
title: Modelle - Übersicht
description: Erfahren Sie, wie Sie in Marketing Campaign Analytics Modelle für maschinelles Lernen erstellen, trainieren, bewerten und verwalten, um Marketing-Ergebnisse zu messen und vorherzusagen.
feature: Models
exl-id: c43d9bc9-4429-45c2-9247-bd24510a24be
autotag-review: '2026-05-01T08:59:10.903Z'
TQID: 'https://experienceleague.adobe.com/T37YTKQlT1mUIfGkJwQkLLGkP0WfTs6jUbZpskPUHgo'
product_v2:
  - id: b88c80e3-31df-4609-989d-d4dac0e6d973
    internal-label: Marketing Campaign Analytics
feature_v2:
  - id: a234aebd-3855-4376-a64d-29b38411e0c5
    internal-label: Marketing mix modeling
  - id: a567f0f7-0057-4079-8ded-5b24cc25af15
    internal-label: Harmonized data
  - id: f40f1683-8300-4054-aab8-77da06ad63ff
    internal-label: Models
  - id: fe1c9ae8-a908-4ae1-a0b6-fcf35177b134
    internal-label: Marketing touch attribution
subfeature_v2:
  - id: a9505d76-24a1-4ffe-bd01-6ac32d5af453
    internal-label: Model insights
  - id: c89e26b6-808d-4500-8b01-450a63466999
    internal-label: Build model
  - id: cb40363e-1205-4921-971c-9ee6bdb18329
    internal-label: Scoring data
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
    internal-label: Admin
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
    internal-label: Reporting
  - id: e1e0219c-f879-479f-8427-888ed2a6e9c2
    internal-label: Insights
  - id: eb30f47f-d87a-400f-8f78-63ce7979ff56
    internal-label: Machine learning
source-git-commit: c75532d37a87f39cb61eabd58333b39895cf3a69
workflow-type: tm+mt
source-wordcount: '1329'
ht-degree: 0%
---
# Modelle - Übersicht

{{mm-mca-rebranding}}

Mit der Modellfunktion in Marketing Campaign Analytics können Sie Modelle konfigurieren, trainieren und bewerten, die speziell auf Ihre Geschäftsziele zugeschnitten sind. Das Training und Scoring unterstützt KI-gestütztes Transferlernen zwischen Multitouch-Attribution und Marketing-Mix-Modellierung.

Die Modelle basieren auf den harmonisierten Daten, die Sie im Rahmen des Programm-Workflows erstellen.

Ein Modell in Marketing Campaign Analytics ist ein maschinelles Lernmodell, mit dem ein bestimmtes Ergebnis anhand von Marketing-Investitionen gemessen und vorhergesagt werden kann. Marketing-Touchpoints und Daten auf Zusammenfassungsebene können als Eingabe verwendet werden. Mit Marketing Campaign Analytics können Sie Varianten von Modellen erstellen, die auf verschiedenen Variablensätzen, Dimensionen und Ergebnissen basieren, z. B. Umsatz, verkaufte Einheiten, Leads.

Ein Modell erfordert:

* Eine Konversion.
* Ein oder mehrere Marketing-Touchpoints (Kanäle), die aus Daten auf Zusammenfassungsebene, Marketing-Touchpoint-Daten (Ereignisdaten) oder beidem bestehen.
* Ein konfigurierbares Lookback-Fenster.
* Ein konfigurierbares Trainings-Fenster.

Ein Modell kann optional Folgendes enthalten:

* Externe Faktoren.
* Interne Faktoren.
* Vorkenntnisse von Marketing-Beiträgen aus anderen Quellen wie Erfahrungen mit früheren Stakeholdern, inkrementelle Tests und andere Modelle.
* Ausgabenanteil, der den relativen Ausgabenanteil als Proxy verwendet, wenn die Marketing-Daten spärlich sind.

Wenn ein Modell zum ersten Mal erstellt wird, startet die Erstellung sofort den Trainings- und Bewertungsprozess. Nach Abschluss des anfänglichen Trainings- und Scoring-Durchgangs stehen Modelleinblicke zur Überprüfung zur Verfügung. Ein Modell wird anschließend neu trainiert. Wenn dem Modell Daten hinzugefügt werden, ist außerdem eine manuelle Neubewertung des Modells erforderlich. Umschulung und Neubewertung sind ein iterativer Prozess, da neue Erkenntnisse und Informationen auftauchen und Anpassungen erforderlich sind, um eine Modellanpassung zu erhalten, die für Ihre Geschäftsziele am besten geeignet ist.

## Vollständige funnel-Modellierung

{{release-limited-testing-section}}

Die vollständige funnel-Modellierung ermöglicht die Modellierung der realen Phasen der funnel. Zum Beispiel von der Newsletter-Anmeldung bis hin zu einem Kauf. Eine vollständige funnel-Modellierung zeigt, wie das Marketing Kunden durch diese funnel bewegt. Die vollständige funnel-Modellierung schreibt den Kanälen der oberen funnel die Konversionen zu, die diese Kanäle nachgelagert beeinflussen, und stimmt die Ergebnisse ab, sodass sich die Beiträge korrekt und ohne Doppelzählung summieren.

Mithilfe der vollständigen funnel-Modellierung können Sie einen oberen und einen unteren funnel-KPI gleichzeitig mit einem unteren funnel-KPI modellieren.

* Beispiele für obere funnel-KPIs sind Newsletter-Anmeldungen und andere Metriken zur Markenwahrnehmung.
* Beispiele für niedrigere funnel-Metriken sind typische Konversionsmetriken wie Umsatz und Bestellungen.

In einem konversionsfokussierten MMM-Modell werden die Taktiken der oberen funnel oft weniger gut bewertet. Die vollständige funnel-Modellierung hilft Ihnen Folgendes zu verstehen:

* Welche Medien- und Marketing-Taktiken zum funnel-Oberziel beigetragen haben.
* Welche Medien- und Marketing-Taktiken haben indirekt zum Ziel der Konversion beigetragen? Die höheren funnel-Modellgewichte sind ein Input für das niedrigere funnel-Modell, um gegebenenfalls den Medien- und Marketing-Taktiken mehr Gewicht zu verleihen.

## Erstellen von Modellen

Verwenden Sie zum Erstellen eines Modells den Schritt-für-Schritt-Konfigurationsablauf für Marketing Campaign Analytics-Modelle, der bei der Auswahl von **[!UICONTROL Open model canvas]** verfügbar ist. Weitere [&#x200B; finden Sie unter &#x200B;](build.md) von Modellen .

## Modelle verwalten

So zeigen Sie eine Tabelle Ihrer aktuellen Modelle in der Benutzeroberfläche von Marketing Campaign Analytics an:

1. Wählen Sie ![FileDataS2](/help/assets/icons2/FileData.svg)-**[!UICONTROL Models]** in der linken Leiste aus.

1. Eine Tabelle der aktuellen Modelle wird angezeigt.

   Die Tabellenspalten geben Details zum Modell an.

   | Spaltenname | Details |
   |---|---|
   | **[!UICONTROL Name]** | Name des Modells. Wenn ein Modell für die vollständige funnel-Modellierung aktiviert ist, wird die [!BADGE &#x200B; „Vollständige funnel&quot; &#x200B;]{type=Informative}. |
   | **[!UICONTROL Description]** | Beschreibung des Modells |
   | **[!UICONTROL Conversion event]** | Die für das Modell ausgewählte Konvertierung. |
   | **[!UICONTROL Run frequency]** | Die Lauffrequenz des Trainings des Modells. |
   | **[!UICONTROL Last run]** | Datum und Uhrzeit des letzten Trainings des Modells. |
   | **[!UICONTROL Status]** | Der Status des Modells. |

   Um die Tabelle in einer beliebigen Spalte in aufsteigender ![ArrowMoveUpS2](/help/assets/icons2/ArrowMoveUp.svg) oder absteigender Reihenfolge ![ArrowMoveDownS2](/help/assets/icons2/ArrowMoveDown.svg) zu sortieren, klicken Sie auf den Titel der Spalte.

   Um die **[!UICONTROL Name]** Spalte zu sortieren oder zu skalieren, wählen Sie **[!UICONTROL Name]** ChevronDown![&#x200B; aus](/help/assets/icons/ChevronDown.svg). Wählen Sie im Kontextmenü **[!UICONTROL Sort ascending]**, **[!UICONTROL Sort descending]** oder **[!UICONTROL Resize column]** aus. Um die Größe der **[!UICONTROL Name]** Spalte zu ändern, bewegen Sie den Mauszeiger über das Spaltentrennzeichen.

   Der gemeldete Status des Modells hängt davon ab, wo sich ein Modell innerhalb seines Lebenszyklus befindet. Ob beispielsweise ein Modell erstellt, erfolgreich (neu) trainiert wurde oder nicht oder ob die Bewertung erfolgreich (neu) erstellt wurde oder nicht.

   In der folgenden Tabelle:

   * ![Häkchen](/help/assets/icons/Checkmark.svg) - zeigt eine erfolgreiche Ausführung eines Schritts im Modelllebenszyklus an.
   * ![Uhr](/help/assets/icons/Clock.svg) - zeigt die aktuelle Ausführung eines Schritts im Modelllebenszyklus an.
   * ![Schließen](/help/assets/icons/Close.svg) - zeigt eine fehlgeschlagene Ausführung eines Schritts im Modelllebenszyklus an.

   | Status | [Build](/help/models/build.md) | [Zug](/help/models/train-score.md#train) | [Ergebnis](/help/models/train-score.md#score) | [Umschulen](/help/models/train-score.md#train) | [Rescore](/help/models/train-score.md#score) |
   |---|:---:|:---:|:---:|:---:|:---:|
   | In Bearbeitung | ![Häkchen](/help/assets/icons/Checkmark.svg) | | | | |
   | In Bearbeitung | ![Häkchen](/help/assets/icons/Checkmark.svg) | ![Uhr](/help/assets/icons/Clock.svg) | | | |
   | In Bearbeitung | ![Häkchen](/help/assets/icons/Checkmark.svg) | ![Häkchen](/help/assets/icons/Checkmark.svg) | ![Uhr](/help/assets/icons/Clock.svg) | | |
   | In Bearbeitung | ![Häkchen](/help/assets/icons/Checkmark.svg) | ![Häkchen](/help/assets/icons/Checkmark.svg) | ![Häkchen](/help/assets/icons/Checkmark.svg) | ![Uhr](/help/assets/icons/Clock.svg) | |
   | In Bearbeitung | ![Häkchen](/help/assets/icons/Checkmark.svg) | ![Häkchen](/help/assets/icons/Checkmark.svg) | ![Häkchen](/help/assets/icons/Checkmark.svg) | ![Häkchen](/help/assets/icons/Checkmark.svg) | ![Uhr](/help/assets/icons/Clock.svg) |
   | Training failed | ![Häkchen](/help/assets/icons/Checkmark.svg) | ![Schließen](/help/assets/icons/Close.svg) | | | |
   | Training failed | ![Häkchen](/help/assets/icons/Checkmark.svg) | ![Häkchen](/help/assets/icons/Checkmark.svg) | ![Häkchen](/help/assets/icons/Checkmark.svg) | ![Schließen](/help/assets/icons/Close.svg) | |
   | Training successful | ![Häkchen](/help/assets/icons/Checkmark.svg) | ![Häkchen](/help/assets/icons/Checkmark.svg) | | | |
   | Training successful | ![Häkchen](/help/assets/icons/Checkmark.svg) | ![Häkchen](/help/assets/icons/Checkmark.svg) | ![Häkchen](/help/assets/icons/Checkmark.svg) | ![Häkchen](/help/assets/icons/Checkmark.svg) | |
   | Bewertung fehlgeschlagen | ![Häkchen](/help/assets/icons/Checkmark.svg) | ![Häkchen](/help/assets/icons/Checkmark.svg) | ![Schließen](/help/assets/icons/Close.svg) | | |
   | Bewertung fehlgeschlagen | ![Häkchen](/help/assets/icons/Checkmark.svg) | ![Häkchen](/help/assets/icons/Checkmark.svg) | ![Häkchen](/help/assets/icons/Checkmark.svg) | ![Häkchen](/help/assets/icons/Checkmark.svg) | ![Schließen](/help/assets/icons/Close.svg) |
   | Bewertung erfolgreich | ![Häkchen](/help/assets/icons/Checkmark.svg) | ![Häkchen](/help/assets/icons/Checkmark.svg) | ![Häkchen](/help/assets/icons/Checkmark.svg) | | |
   | Bewertung erfolgreich | ![Häkchen](/help/assets/icons/Checkmark.svg) | ![Häkchen](/help/assets/icons/Checkmark.svg) | ![Häkchen](/help/assets/icons/Checkmark.svg) | ![Häkchen](/help/assets/icons/Checkmark.svg) | ![Häkchen](/help/assets/icons/Checkmark.svg) |

   {style="table-layout:fixed"}

1. Um die für die Liste angezeigten Spalten zu ändern, wählen Sie ![Spalteneinstellungen](/help/assets/icons/ColumnSetting.svg) aus und schalten Sie die Spalten ein ![Aktivieren](/help/assets/icons/Checkmark.svg) oder aus.

Sie können die folgenden Aktionen für ein bestimmtes Modell ausführen.

### Modelleinblicke

Die Funktion Modelleinblicke ist nur für erfolgreich trainierte und bewertete Modelle verfügbar.

So zeigen Sie die Insights eines Modells an:

1. Wählen Sie ![FileData](/help/assets/icons/FileData.svg)-**[!UICONTROL Models]** in der linken Leiste aus.
1. Wählen Sie den Modellnamen.

Sie werden zu &quot;[&#x200B; Insights“ &#x200B;](insights.md).

### Details anzeigen

So zeigen Sie weitere Details zu einem Modell an:

1. Wählen Sie ![FileData](/help/assets/icons/FileData.svg)-**[!UICONTROL Models]** in der linken Leiste aus.

1. Wählen Sie ![Info](/help/assets/icons/Info.svg) für ein Modell aus, um ein Popup mit Details wie **[!UICONTROL Description]**, **[!UICONTROL Run frequency]**, **[!UICONTROL Last run status]**, **[!UICONTROL Spend share]** und mehr anzuzeigen.




### Duplizieren

Sie können ein Modell schnell duplizieren.

1. Wählen Sie ![FileData](/help/assets/icons/FileData.svg)-**[!UICONTROL Models]** in der linken Leiste aus.

1. Wählen Sie ![Mehr](/help/assets/icons/More.svg) für ein Modell aus und wählen Sie im Kontextmenü **[!UICONTROL Duplicate]** aus.

Sie werden zu den Schritten zum Erstellen eines neuen Modells weitergeleitet, wobei ein vorgeschlagener Name aus dem Namen des ursprünglichen Modells mit **[!UICONTROL (Copy)] (_)_ wird**.

### Bearbeiten

Sie können den Namen, die Beschreibung und den Zeitplan für das Training und die Bewertung eines Modells bearbeiten.

1. Wählen Sie ![FileData](/help/assets/icons/FileData.svg)-**[!UICONTROL Models]** in der linken Leiste aus.

1. Wählen Sie ![Mehr](/help/assets/icons/More.svg) für ein Modell aus und wählen Sie im Kontextmenü **[!UICONTROL Edit]** aus.

   Im Dialogfeld **[!UICONTROL Edit model]** :

   ![Modell bearbeiten](../assets/model-edit.png)

   * Geben Sie einen neuen **[!UICONTROL Name]** und eine neue **[!UICONTROL Description]** ein.

   * Um die Zeitplanung zu aktivieren, aktivieren Sie **[!UICONTROL Enable schedule model training and scoring]**. Sie können die Planung nur für Modelle aktivieren, die trainiert und bewertet wurden.

     1. **[!UICONTROL Scoring frequency]** auswählen:

        * **[!UICONTROL Daily]**: Geben Sie eine gültige Zeit ein (z. B. `10:00 am`) oder verwenden Sie ![Uhr](/help/assets/icons/Clock.svg), um die Zeit festzulegen.
        * **[!UICONTROL Weekly]**: Wählen Sie einen Wochentag aus und geben Sie eine gültige Zeit ein (z. B. `10:00 am`) oder verwenden Sie ![Uhr](/help/assets/icons/Clock.svg), um die Zeit festzulegen.
        * **[!UICONTROL Monthly]**: Wählen Sie bei jedem Dropdown-Menü einen Tag des Monats aus und geben Sie eine gültige Zeit ein (z. B. `10:00 am`) oder verwenden Sie ![Uhr](/help/assets/icons/Clock.svg), um die Zeit festzulegen.

     1. Wählen Sie eine **[!UICONTROL Training frequency]** aus dem Dropdown-Menü aus: **[!UICONTROL Monthly]**, **[!UICONTROL Quarterly]**, **[!UICONTROL Yearly]** oder **[!UICONTROL None]**.

   * Wenn das vollständige funnel-Modell aktiviert ist, wird eine deaktivierte Option Vollständige funnel-Attribution aktivieren angezeigt. Diese Einstellung kann nicht geändert werden.

   * Um [Bewertungsdaten für Customer Journey Analytics verfügbar zu machen](build.md#customer-journey-analytics) wählen Sie **[!UICONTROL Enable scores for Customer Journey Analytics]** aus.

     Sobald die Bewertungen für Customer Journey Analytics aktiviert wurden, können Sie diese Einstellung nur deaktivieren, wenn das Modell gelöscht wird.

   * So aktualisieren Sie die [Berichtsfelder für granulare Insights](/help/models/build.md#granular-insights-reporting-fields) im **[!UICONTROL Granular Insights Reporting Fields]** Abschnitt:
     1. Wählen Sie ein oder mehrere harmonisierte Felder aus dem **[!UICONTROL _Harmonisierte Felder auswählen_]** unter **[!UICONTROL Includes]** aus. Die ausgewählten harmonisierten Felder werden dem Bedienfeld hinzugefügt.
     1. Wählen Sie **[!UICONTROL *Harmonisiertes Feld *]**![CrossSize100](/help/assets/icons/CrossSize100.svg) aus, um ein harmonisiertes Feld aus dem Container mit den ausgewählten harmonisierten Feldern zu entfernen.
     1. Wählen Sie **[!UICONTROL Clear all]** aus, um alle ausgewählten harmonisierten Felder zu entfernen.

     >[!IMPORTANT]
     >Jedes Modell mit MTA, das vor dem 12. Januar 2026 erstellt wurde, sollte dupliziert werden, um granulare Modelleinblicke zu ermöglichen.<br/>
     >Eine Bewertung ist für jedes vorhandene Modell erforderlich, um die aktualisierten granularen Dimensionen in den Bewertungsdaten widerzuspiegeln.
     >

1. Wählen Sie **[!UICONTROL Save]** aus.

### trainieren

Trainieren Sie ein Modell neu, wenn Sie neue inkrementelle Marketing- und Faktordaten einbeziehen möchten. Weitere Informationen finden [&#x200B; unter &#x200B;](train-score.md#train) trainieren und bewerten .

### Ergebnis

Sie können ein Modell inkrementell auf der Grundlage neuer Marketing-Daten bewerten oder ein Modell für einen bestimmten Datumsbereich neu bewerten. Weitere Informationen finden [&#x200B; unter &#x200B;](train-score.md#score) trainieren und bewerten .

### Modelle löschen

Löschen eines Modells:

1. Wählen Sie ![FileData](/help/assets/icons/FileData.svg)-**[!UICONTROL Models]** in der linken Leiste aus.
1. Wählen Sie ![Mehr](/help/assets/icons/More.svg) für ein Modell aus und wählen Sie im Kontextmenü **[!UICONTROL Delete]** aus. Wählen Sie alternativ ![&#x200B; blaue Aktionsleiste &#x200B;](/help/assets/icons/Delete.svg)Löschen“ **[!UICONTROL Delete]**.
1. Wählen Sie **[!UICONTROL Delete]** im Bestätigungsdialogfeld **[!UICONTROL Delete model]** aus, um das Modell zu löschen. Wählen Sie zum Abbrechen **[!UICONTROL Cancel]** aus.

So löschen Sie mehrere Modelle:

1. Mehrere Modelle auswählen.
1. Wählen Sie in der blauen Aktionsleiste die Option ![Löschen](/help/assets/icons/Delete.svg) aus, **[!UICONTROL Delete]** die Modelle zu löschen.
1. Wählen Sie **[!UICONTROL Delete]** im Bestätigungsdialogfeld **[!UICONTROL Delete *x *-Modelle]**, um die Modelle zu löschen. Wählen Sie zum Abbrechen **[!UICONTROL Cancel]**&#x200B;aus.

