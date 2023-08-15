# Action On Projectile Land
[Power Types](../power_types.md)

Executes an Entity Action and a Block Action at the location that a thrown projectile lands.

Type ID: `ra_additions:action_on_projectile_land`
### Fields
 | Field | Type | Default | Description | 
|---|---|---|---|
 | `projectile` | [Identifier](../data_types/identifier.md) | _optional_ | The identifier of the projectile entity. | 
 | `should_damage` | [Boolean](../data_types/boolean.md) | _optional_ | Determines if the entity will be damaged by the projectile. | 
 | `bientity_action` | [Bientity Action](../bientity_action_types.md) | _optional_ | The bientity action to be executed between the entity hit, and the entity with this power. | 
 | `bientity_condition` | [Bientity Condition](../bientity_condition_types.md) | _optional_ | If specified, only execute the bientity action if this condition is fulfilled. | 
 | `block_action` | [Block Action](../block_action_types.md) | _optional_ | The block action to be executed if specified. | 
 | `block_condition` | [Block Condition](../block_condition_types.md) | _optional_ | If specified, only execute the specified actions if the block condition is fulfilled. | 

### Example
```json
{
  "type": "ra_additions:action_on_projectile_land",
  "should_damage": false,
  "bientity_action": {
    "type": "apoli:target_action",
    "action": {
      "type": "apoli:execute_command",
      "command": "spreadplayers ~ ~ 1 3 false @s"
    }
  },
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
This example will make it so that any projectile that you throw, that lands on a coal block, will become a diamond block.
