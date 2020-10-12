---
title: "macOSAssociatedDomainsKeyValuePair resource type"
description: "Key value pair for associated domains"
author: "dougeby"
localization_priority: Normal
ms.prod: "intune"
doc_type: resourcePageType
---

# macOSAssociatedDomainsKeyValuePair resource type

Namespace: microsoft.graph

> **Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.

> **Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.

Key value pair for associated domains


Inherits from [keyValuePair](../resources/intune-shared-keyvaluepair.md)

## Properties
|Property|Type|Description|
|:---|:---|:---|
|name|String|Name for this key-value pair Inherited from [keyValuePair](../resources/intune-shared-keyvaluepair.md)|
|value|String|Value for this key-value pair Inherited from [keyValuePair](../resources/intune-shared-keyvaluepair.md)|

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.macOSAssociatedDomainsKeyValuePair"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.macOSAssociatedDomainsKeyValuePair",
  "name": "String",
  "value": "String"
}
```






