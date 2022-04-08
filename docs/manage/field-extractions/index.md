---
slug: /manage/field-extractions
---

# Field Extractions

Field extractions allow you to parse [fields] (Fields.md "Fields") from your log messages at the time the messages are ingested, which eliminates the need to parse fields at the query level. With Field Extraction Rules (FERs) in place, users can use the pre-parsed fields for ad-hoc searches, scheduled searches, real-time alerts, and dashboards. In addition, field extraction rules help standardize field names and searches, simplify the search syntax and scope definition, and improve search performance. 

Fields are extracted from the time you create your FER moving forward. Therefore, set your FERs early on to take advantage of this automatic parsing mechanism.

For best practices on naming your fields, see [Field Naming Convention](field-naming-convention.md). 

:::important
You need the **Manage field extraction rules** [role capability] (Users-and-Roles/Manage-Roles/05-Role-Capabilities.md "Role Capabilities") to create a field extraction rule. 
:::

![FER page.png](/img/field-extraction-rules/fer-page.png)

The **Manage Data** \> **Logs** \> **Field Extraction Rules** page displays the following information: 

When hovering over a row in the table there are icons that appear on the far right for editing, disabling and deleting the rule.

* **Status** shows a checkmark in a green circle ![check in green circle.png](/img/reuse/check-green-circle.png) to indicate if the Rule is actively being applied or an exclamation mark in a red circle ![exclamation in red circle.png](/img/reuse/exclamation-red-circle.png) to indicate if the Rule is disabled.
* **Rule Name**
* **Applied At** indicates when the field extraction process occurs, either at Ingest or Run time.
* **Scope** 
* **Created** date and time by user
* **Last Modified** date and time by user
* **Fields Capacity** (bottom of table) shows how many fields your account is using, out of the total available for use.

You can view the fields created in your account and what features are referencing them on the [Fields] (Fields.md "Fields") page.

On the **Manage Data** \> **Logs** \> **Field Extraction Rules** page you can:

* Click **+ Add** to [create a Field Extraction Rule](create-field-extraction-rule.md).
* Search Field Extraction Rules by name and scope.
* [**Edit** a Field Extraction Rule](edit-field-extraction-rules.md).
* **Disable** a Field Extraction Rule.
* **Delete** a Field Extraction Rule.

## Limitations
FIX
{@import ../../reuse/fer-limitations.md}

## Micro Lesson: Field Extraction Rules Basics

<Iframe url="https://www.youtube.com/embed/Xv3pSwhVCN4"
        width="854px"
        height="480px"
        id="myId"
        className="video-container"
        display="initial"
        position="relative"
        allow="accelerometer; autoplay=1; clipboard-write; encrypted-media; gyroscope; picture-in-picture" 
        allowfullscreen
        />

import Iframe from 'react-iframe';

## Edit a Field Extraction Rule

Changes to Field Extraction Rules are implemented immediately.

1.  In Sumo Logic, go to **Manage Data** \> **Logs** \> **Field Extraction Rules.**
2.  Find the rule in the table and click it. A window appears on the right of the table, click the **Edit** button.
3.  Make changes as needed and click **Save** when done.

## Delete a Field Extraction Rule

Deleting a Field Extraction Rule doesn't delete the fields it was parsing. You can delete any unwanted fields on the [Fields] (Fields.md "Fields") page.

1.  In Sumo Logic, go to **Manage Data** \> **Logs** \> **Field Extraction Rules.**
2.  Find the rule to delete in the table and click it. A window appears on the right of the table, click the **More Actions** button, and select **Delete**.

import DocCardList from '@theme/DocCardList';
import {useCurrentSidebarCategory} from '@docusaurus/theme-common';

## Guide contents

In this section, we will introduce the following concepts:

<DocCardList items={useCurrentSidebarCategory().items}/>