---
title: "managedAppStatus resource type"
description: "Represents app protection and configuration status for the organization."
author: "tfitzmac"
localization_priority: Normal
ms.prod: "intune"
---

# managedAppStatus resource type

> **Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change. Use of these APIs in production applications is not supported.

> **Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.

Represents app protection and configuration status for the organization.
## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List managedAppStatuses](../api/intune-mam-managedappstatus-list.md)|[managedAppStatus](../resources/intune-mam-managedappstatus.md) collection|List properties and relationships of the [managedAppStatus](../resources/intune-mam-managedappstatus.md) objects.|
|[Get managedAppStatus](../api/intune-mam-managedappstatus-get.md)|[managedAppStatus](../resources/intune-mam-managedappstatus.md)|Read properties and relationships of the [managedAppStatus](../resources/intune-mam-managedappstatus.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|displayName|String|Friendly name of the status report.|
|id|String|Key of the entity.|
|version|String|Version of the entity.|

## Relationships
None
## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedAppStatus"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedAppStatus",
  "displayName": "String",
  "id": "String (identifier)",
  "version": "String"
}
```





