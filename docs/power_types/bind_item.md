# Bind Item
[Power Types](../power_types.md)

Makes certain items unable to leave in the entity's inventory until death.

Type ID: `ra_additions:bind_item`
### Fields
 | Field | Type | Default | Description | 
|---|---|---|---|
 | `item_condition` | [Item Condition](../item_condition_types.md) | _optional_ | If specified, only make the items that fulfill the specified item condition are unable to leave the players inventory. | 
 | `prevent_use_condition` | [Item Condition](../item_condition_types.md) | _optional_ | If specified, it won't let the player use the items that fulfill the specified item condition. | 
 | `slots` | [Array](../data_types/array.md) of [Int](../data_types/int.md) | _optional_ | If specified, only make the items that are in the listed inventory slots are unable to leave the players inventory. See the "Item Stack Slot" column of [Positioned Item Stack Slots](https://origins.readthedocs.io/en/latest/misc/extras/positioned_item_stack_slots/) for possible values. | 

### Example
```json
{
  "type": "ra_additions:bind_item",
  "item_condition": {
    "type": "apoli:ingredient",
    "ingredient": {
      "item": "minecraft:trident"
    }
  },
  "prevent_use_condition": {
    "type": "apoli:ingredient",
    "ingredient": {
      "item": "minecraft:trident"
    }
  }
}
```
This example would make it so that any trident that enters your inventory can't leave it until death, and can't be thrown.
