---
title: "reviewSetQuery resource type"
description: "Review set queries are used to query and cull data stored in an eDiscovery reviewSet"
localization_priority: Normal
author: "mahage-msft"
ms.prod: "compliance"
doc_type: "resourcePageType"
---

# reviewSetQuery resource type

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Review set queries are used to query and cull data stored in an eDiscovery [reviewSet](reviewset.md).

## Methods

| Method       | Return Type | Description |
|:-------------|:------------|:------------|
| [List](../api/reviewsetquery-list.md) | [reviewSetQuery](reviewsetquery.md) collection | List the review set queries in a review set. |
| [Create](../api/reviewsetquery-post.md) | [reviewSetQuery](reviewsetquery.md) | Create a new review set query. |
| [Get](../api/reviewsetquery-get.md) | [reviewSetQuery](reviewsetquery.md) | Read the properties and relationships of a **reviewSetQuery** object. |
| [Update](../api/reviewsetquery-update.md) | None | Update a review set query. |
| [Delete](../api/reviewsetquery-delete.md) | None | Delete review set query. |

## Properties

| Property     | Type        | Description |
|:-------------|:------------|:------------|
| createdBy | [identitySet](/graph/api/resources/identityset) | The user who created the query. |
| createdDateTime |DateTimeOffset| The time and date when the query was created. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`|
| displayName | String | The name of the query|
| id |String| The unique identifier of the query. Read-only.|
| lastModifiedBy | [identitySet](/graph/api/resources/identityset) | The user who last modified the query. |
| lastModifiedDateTime |DateTimeOffset | The date and time the query was last modified. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`|
| query | String | The query string in KQL (Keyword Query Language) query. Please refer to https://docs.microsoft.com/microsoft-365/compliance/document-metadata-fields-in-advanced-ediscovery for more details.  This field maps directly to the keywords condition.  You can refine searches by using fields listed in the *searchable field name* paired with values, e.g. *subject:"Quarterly Financials" AND Date>=06/01/2016 AND Date<=07/01/2016* |

## Relationships

None.

## JSON representation

The following is a JSON representation of the resource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.reviewSetQuery",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
  "createdBy": "String",
  "createdDateTime": "String (timestamp)",
  "displayName": "String",
  "id": "String (identifier)",
  "lastModifiedBy": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "query": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "reviewSetQuery resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->