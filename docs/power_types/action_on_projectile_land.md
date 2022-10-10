# Action On Projectile Land

[Power Type](../power_types.md)

Executes an Entity Action and a Block Action at the location that a thrown projectile lands.

Type ID: `ra_additions:action_on_projectile_land`

### Fields

Field | Type | Default | Description
------|------|---------|-------------
`projectile` | [Identifier](../data_types/identifier.md) | _optional_ | The identifier of the projectile entity.
`entity_action` | [Entity Action Type](https://origins.readthedocs.io/en/latest/types/entity_action_types/) | _optional_ | The entity action to be executed on the projectile if specified.
`self_action` | [Entity Action Type](https://origins.readthedocs.io/en/latest/types/entity_action_types/) | _optional_ | The entity action to be executed on the player if specified.
`block_action` | [Block Action Type](https://origins.readthedocs.io/en/latest/types/block_action_types/) | _optional_ | The block action to be executed if specified.
`block_condition` | [Block Condition Type](https://origins.readthedocs.io/en/latest/types/block_condition_types/) | _optional_ | If specified, only execute the specified actions if the block condition is fulfilled.

### Example
```json
{
	"type": "ra_additions:action_on_projectile_land",
	"block_action": {
		"type": "apoli:set_block",
		"block": "minecraft:diamond_block"
	},
	"block_condition": {
		"type": "apoli:block",
		"block": "minecraft:coal_block"
	}
}
```
When any projectile lands, if the block it lands on is a coal block, turn it into a diamond block.
