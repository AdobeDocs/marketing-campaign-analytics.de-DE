---
title: Administration
description: Erfahren Sie, wie Sie Marketing Campaign Analytics verwalten.
feature: Administration
exl-id: 76d6d15d-a838-4ee2-9929-e55ea8946b80
autotag-review: '2026-05-01T09:07:55.299Z'
TQID: 'https://experienceleague.adobe.com/GZOR-NsylnAmpFEuZNDpvF0Br8eL-HKGYIPUBs00sNQ'
product_v2:
  - id: b88c80e3-31df-4609-989d-d4dac0e6d973
    internal-label: Marketing Campaign Analytics
feature_v2:
  - id: a567f0f7-0057-4079-8ded-5b24cc25af15
    internal-label: Harmonized data
  - id: d822825b-9821-40d5-9b0d-42a9e3f317c5
    internal-label: Plans
  - id: e0abf868-dae2-4c1c-83e9-b21799232845
    internal-label: Datasets
  - id: f40f1683-8300-4054-aab8-77da06ad63ff
    internal-label: Models
  - id: f6633d1c-3d2d-4f48-95d4-4bbc9913db52
    internal-label: Data governance
  - id: fbd94e4b-f9b8-42a4-8df5-3f917aabae24
    internal-label: Schemas
  - id: fe2edbb1-46f9-4347-a27c-577cab3640cb
    internal-label: Administration
subfeature_v2:
  - id: abe9e290-7d2f-4131-b71e-ef9900865044
    internal-label: Access control
  - id: a6da0571-746e-4d59-89a4-7b691b1c3b9a
    internal-label: Architecture
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
    internal-label: Admin
topic_v2:
  - id: b23e006f-0a29-4f1d-8fd0-77aa56f3d12b
    internal-label: Data modeling
  - id: c7d04a2c-412a-4c9d-9d7a-4456eaa5adeb
    internal-label: Governance
  - id: ebde5b41-29c9-4f5e-9ef6-1197e85409e3
    internal-label: Data management
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
  - id: f4e6943a-c91a-4134-a2c7-f4f20cfff2f0
    internal-label: Privacy
source-git-commit: 9d6bd798e97d36d49b7753dc9574b102efb3d6bf
workflow-type: tm+mt
source-wordcount: '201'
ht-degree: 6%
---
# Administration

{{mm-mca-rebranding}}

Verwenden Sie die [Adobe Admin Console](https://helpx.adobe.com/de/enterprise/using/admin-console.html), um Marketing Campaign Analytics-Produkte und -Benutzer zu verwalten.

Damit Marketing Campaign Analytics ordnungsgemäß funktioniert, müssen Sie die richtigen Berechtigungen festlegen.

In der Adobe Experience Cloud-Benutzeroberfläche:

1. Wählen Sie **[!UICONTROL Permissions]** in der linken Leiste unter **[!UICONTROL ADMINISTRATION]** aus.

1. Wählen Sie ![&#x200B; linken Bedienfeld &#x200B;](/help/assets/icons/User.svg)Benutzer **[!UICONTROL Roles]** aus.

1. Wählen Sie eine vorhandene Rolle aus oder erstellen Sie eine Rolle mithilfe von **[!UICONTROL Create role]** (z. B. **Marketing Campaign Analytics**) Wenn Sie eine vorhandene Rolle auswählen, klicken Sie auf ![Bearbeiten](/help/assets/icons/Edit.svg) **[!UICONTROL Edit]**, um die Berechtigungen für die Rolle zu bearbeiten. Weitere Informationen finden [&#x200B; unter &#x200B;](https://helpx.adobe.com/de/enterprise/using/admin-console.html) von Rollen .

1. Stellen Sie sicher, dass Sie eine oder mehrere Sandboxes für die Rolle ausgewählt haben.

1. Fügen Sie die **Adobe Marketing Campaign Analytics**-Ressource zur Liste der Ressourcen für die Rolle hinzu.

1. Stellen Sie sicher, dass Sie die richtigen **[!UICONTROL Adobe Marketing Campaign Analytics]** für die Rolle auswählen, die Sie konfigurieren. Sie können eine oder mehrere der folgenden Rollen auswählen:

   - **[!UICONTROL View Adobe Marketing Campaign Analytics Harmonized Data]**
   - **[!UICONTROL Manage Adobe Marketing Campaign Analytics Harmonized Data]**
   - **[!UICONTROL View Adobe Marketing Campaign Analytics Models Configuration]**
   - **[!UICONTROL Manage Adobe Marketing Campaign Analytics Models Configuration]**
   - **[!UICONTROL View Adobe Marketing Campaign Analytics Plans Configuration]**
   - **[!UICONTROL Manage Adobe Marketing Campaign Analytics Plans Configuration]**

     ![Marketing Campaign Analytics RBAC](/help/assets/mix-modeler-rbac.png)


1. Stellen Sie sicher, dass Sie zusätzliche Berechtigungen für die Rolle auswählen. Um beispielsweise Datensätze und Schemata anzuzeigen oder zu verwalten, wählen Sie:

   - **[!UICONTROL Data Management]**: Wählen Sie die entsprechenden Optionen aus: **[!UICONTROL View Datasets]** oder **[!UICONTROL Manage Datasets]**.

   - **[!UICONTROL Data Modeling]**: Wählen Sie die entsprechenden Optionen aus: **[!UICONTROL Manage Schemas]** oder **[!UICONTROL View Schemas]**.

   <!--
    * **[!UICONTROL Data Governance]**: ensure you select **[!UICONTROL View User Activity Log]** and **[!UICONTROL View Data Usage Policies]**.
    -->

   <!--![Permissions](assets/permissions-including-privacy.png)-->

   Wählen Sie **[!UICONTROL Save]** aus, um die Berechtigungen zu speichern.

1. Fügen Sie in **[!UICONTROL Details]** in **[!UICONTROL Role]** die entsprechenden **[!UICONTROL Users]** oder **[!UICONTROL User groups]** hinzu, um Benutzenden Zugriff auf Marketing Campaign Analytics zu gewähren.
