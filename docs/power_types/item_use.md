# Item Use

[Power Type](../power_types.md).

This power uses the existing item interaction system in Minecraft to execute actions. which means that when used, the actions won't happen if something of higher priority occurs (for example opening a chest).

Type ID: `ra_additions:item_use`

### Fields

Field  | Type | Default | Description
-------|------|---------|-------------
`cooldown` | [Integer](../data_types/integer.md) | `0` | Sets a cooldown on the item (Similar to ender pearl cooldowns).
`entity_action` | [Entity Action Type](https://origins.readthedocs.io/en/latest/types/entity_action_types/) | _optional_ | The entity action to be executed on the player if specified.
`item_action` | [Item Action Type](https://origins.readthedocs.io/en/latest/types/item_action_types/) | _optional_ | The item action to be executed if specified.
`item_condition` | [Item Condition Type](https://origins.readthedocs.io/en/latest/types/item_condition_types/) | _optional_ | If specified, only execute the action if the item condition is fulfilled.

### Example
```json
{
	"type": "ra_additions:item_use",
	"cooldown": 20,
	"item_action": {
		"type": "apoli:damage",
		"amount": 1
	}
}
```
Upon right clicking an item while having this power, it will use 1 durability, and put that item on cooldown for 20 seconds.
