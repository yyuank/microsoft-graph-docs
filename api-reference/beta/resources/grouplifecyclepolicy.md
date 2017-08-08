# groupLifecyclePolicy resource type

Represents a a lifecycle policy for an Office 365 group. A group lifecycle policy allows administrators to set an expiration period for groups. For example, after 180 days, a group expires. When a group reaches it's expiration, owners of the group are required to renew their group within a time interval defined by the administrator. Once renewed, the group expiration is extended by the number of days defined in the policy. For example, the group's new expiration is 180 days after renewal. If the group is not renewed, it expires and is deleted. The group can be restored within a period of 30 days from deletion.

## Methods

| Method | Return Type | Description |
|:---------------|:--------|:----------|
|[Get groupLifecyclePolicy](../api/grouplifecyclepolicy_get.md) | [groupLifecyclePolicy](grouplifecyclepolicy.md) |Read properties and relationships of a groupLifecyclePolicy object.|
|[List groupLifecyclePolicies](../api/grouplifecyclepolicy_list.md) | [groupLifecyclePolicy](grouplifecyclepolicy.md) collection | List all the groupLifecyclePolicies. |
|[Update groupLifecyclePolicy](../api/grouplifecyclepolicy_update.md) | [groupLifecyclePolicy](grouplifecyclepolicy.md)	| Updates a groupLifecyclePolicy object. |
|[Delete groupLifecyclePolicy](../api/grouplifecyclepolicy_delete.md) | None | Deletes a groupLifecyclePolicy object. |
|[Add a group to a groupLifecyclePolicy](../api/grouplifecyclepolicy_addgroup.md)|None| Adds a group to a lifecycle policy |
|[Remove a group from a groupLifecyclePolicy](../api/grouplifecyclepolicy_removegroup.md)|None| Removes a group to a lifecycle policy. |
|[Renew a group](../api/grouplifecyclepolicy_renewgroup.md)|None| Renews a group's expiration date. |

## Properties

| Property | Type | Description |
|:---------------|:--------|:----------|
|alternateNotificationEmails|String| List of email address to send notifications for groups without owners. Multiple email address can be defined by separating email address with a semicolon. |
|groupLifetimeInDays|Int32| Number of days before a group expires and needs to be renewed. Once renewed, the group expiration is extended by the number of days defined. |
|id|Guid| A unique identifier for a policy. Read-only.|
|managedGroupTypes|String| The group type for which the expiration policy applies. Possible values are **All**, **Selected** or **None**. |

## Relationships

None

## JSON representation

Here is a JSON representation of the resource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.groupLifecyclePolicy"
}-->

```json
{
  "alternateNotificationEmails": "String",
  "groupLifetimeInDays": 180,
  "id": "Guid (identifier)",
  "managedGroupTypes": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "groupLifecyclePolicy resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->