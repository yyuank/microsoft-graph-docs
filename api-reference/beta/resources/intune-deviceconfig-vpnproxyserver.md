---
title: "vpnProxyServer resource type"
description: "VPN Proxy Server."
author: "tfitzmac"
localization_priority: Normal
ms.prod: "intune"
---

# vpnProxyServer resource type

> **Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change. Use of these APIs in production applications is not supported.

> **Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.

VPN Proxy Server.
## Properties
|Property|Type|Description|
|:---|:---|:---|
|automaticConfigurationScriptUrl|String|Proxy's automatic configuration script url.|
|address|String|Address.|
|port|Int32|Port. Valid values 0 to 65535|

## Relationships
None
## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.vpnProxyServer"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.vpnProxyServer",
  "automaticConfigurationScriptUrl": "String",
  "address": "String",
  "port": 1024
}
```





