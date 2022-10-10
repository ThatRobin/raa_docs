### Modify Item

Applies an item modifier to the item stack with a player fulfilling the "this" criteria.

Type ID: `ra_additions:modify_item`

!!! note

    The player is currently random, and won't reflect the player executing the action due to how apoli item actions work internally. This action is used in cases that require a players existance, but doesnt require a specific player. Such as using a storage to set lore text. 

### Fields:

Field  | Type | Default | Description
-------|------|---------|-------------
`modifier` | [Identifier]((../data_types/identifier.md) |  |  The ID of an item modifier.

### Example

```json
"item_action": {
    "type": "ra_additions:modify_item",
    "modifier": "example:stuff"
}
```
This example will apply the example:stuff (`data/example/item_modifiers/stuff.json`) item modifier to the item stack.
```json
{
    "function": "minecraft:set_lore",
    "entity": "this",
    "lore": [
        {
            "text": "Hello, I'm a custom lore line for your item :]",
            "color": "light_purple",
            "italic": false
        }
    ]
}
```
This being the contents of the example:stuff (`data/example/item_modifiers/stuff.json`) item modifier.