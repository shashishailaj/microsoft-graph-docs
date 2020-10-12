---
title: printerShare resource type
description: Represents a printer that is intended to be discoverable by users and printing applications.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
---

# printerShare resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Represents a printer that is intended to be discoverable by users and printing applications.

## Methods

| Method       | Return Type | Description |
|:-------------|:------------|:------------|
| [List](../api/print-list-shares.md) | [printerShare](printershare.md) collection | Get a list of printer shares in the tenant. |
| [Get](../api/printershare-get.md) | [printerShare](printershare.md) | Read properties and relationships of a **printerShare** object. |
| [Update](../api/printershare-update.md) | [printerShare](printershare.md) | Update a **printerShare** object. |
| [Delete](../api/printershare-delete.md) | None | Unshare a printer. |
| [List allowedUsers](../api/printershare-list-allowedusers.md) | [printUserIdentity](printuseridentity.md) collection | Retrieve a list of users who have been granted access to submit print jobs to the associated printer share. |
| [Add allowedUser](../api/printershare-post-allowedusers.md) | None | Grant the specified user access to submit print jobs to the associated printer share. |
| [Remove allowedUser](../api/printershare-delete-alloweduser.md) | None | Revoke printer share access from the specified user. |
| [List allowedGroups](../api/printershare-list-allowedgroups.md) | [printIdentity](printidentity.md) collection | Retrieve a list of groups that have been granted access to submit print jobs to the associated printer share. |
| [Add allowedGroup](../api/printershare-post-allowedgroups.md) | None | Grant the specified group access to submit print jobs to the associated printer share. |
| [Remove allowedGroup](../api/printershare-delete-allowedgroup.md) | None | Revoke printer share access from the specified group. |

## Properties
| Property     | Type        | Description |
|:-------------|:------------|:------------|
|id|String| The printerShare's identifier. Read-only.|
|displayName|String|The name of the printer share that print clients should display.|
|createdDateTime|DateTimeOffset|The DateTimeOffset when the printer share was created. Read-only.|
|manufacturer|String|The manufacturer reported by the printer associated with this printer share. Read-only.|
|model|String|The model name reported by the printer associated with this printer share. Read-only.|
|isAcceptingJobs|Boolean|Whether the printer associated with this printer share is currently accepting new print jobs.|
|defaults|[printerDefaults](printerdefaults.md)|The default print settings of the printer associated with this printer share.|
|capabilities|[printerCapabilities](printercapabilities.md)|The capabilities of the printer associated with this printer share.|
|location|[printerLocation](printerlocation.md)|The physical and/or organizational location of the printer associated with this printer share.|
|status|[printerStatus](printerstatus.md)|The processing status, including any errors, of the printer associated with this printer share. Read-only.|
|allowAllUsers|Boolean|If true, all users and groups will be granted access to this printer share. This supersedes the allow lists defined by the **allowedUsers** and **allowedGroups** navigation properties.|

## Relationships
| Relationship | Type        | Description |
|:-------------|:------------|:------------|
|printer|[printer](printer.md)|The printer that this printer share is related to. |
|allowedUsers|[printUserIdentity](printuseridentity.md) collection|The users who have access to print using the printer.|
|allowedGroups|[printIdentity](printidentity.md)|The groups whose users have access to print using the printer.|
|jobs|[printJob](printjob.md) collection| The list of jobs that are queued for printing by the printer associated with this printer share.|

## JSON representation

The following is a JSON representation of the resource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.printerShare",
  "keyProperty": "id",
  "baseType":"microsoft.graph.entity"
}-->

```json
{
  "id": "String (identifier)",
  "name": "String",
  "createdDateTime": "String (timestamp)"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "printerShare resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


