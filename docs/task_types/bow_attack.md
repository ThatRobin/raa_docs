# Bow Attack
[Task Types](../task_types.md)

A goal that allows its mob to attack using its bow, if one if found.

Type ID: `ra_additions:bow_attack`
### Fields
 | Field | Type | Default | Description | 
|---|---|---|---|
 | `priority` | [Int](../data_types/int.md) | _optional_ | The priority of the goal, the lower, the more important. | 
 | `speed` | [Double](../data_types/double.md) | _optional_ | The speed it should move to its target | 
 | `attack_interval` | [Int](../data_types/int.md) | _optional_ | The amount of ticks between attacks | 
 | `range` | [Float](../data_types/float.md) | _optional_ | The range the entity must be in to be attacked. | 
 | `bientity_condition` | [Bientity Condition](../bientity_condition_types.md) | _optional_ | A condition to see if it can attack its target. | 

### Example
```json
{
  "type": "ra_additions:bow_attack",
  "priority": 0,
  "speed": 1,
  "attack_interval": 20,
  "range": 15,
  "bientity_condition": {
    "type": "apoli:target_condition",
    "condition": {
      "type": "apoli:entity_type",
      "entity_type": "minecraft:creeper"
    }
  }
}
```

