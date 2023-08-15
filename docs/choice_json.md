# Choice JSON Format
This is the format of a JSON file describing a choice. They need to be placed inside the `choices` folder within your namespace.

 | Fields | Type | Default | Description | 
|---|---|---|---|
 | `powers` | [Array](data_types/array.md) of [Identifiers](data_types/identifier.md) | _optional_ | IDs of the powers this choice should have. | 
 | `icon` | [Item Stack](data_types/item_stack.md) | _optional_ | The item stack which is displayed as the icon for the description button for the choice. | 
 | `name` | [String](data_types/string.md) | _optional_ | The display name of the choice. | 
 | `description` | [String](data_types/string.md) | _optional_ | The description of the choice. | 
 | `action_on_chosen` | [Entity Action Type](entity_action_types.md) | _optional_ | The action that is run when they player selects this choice. | 

### Examples
```json
{
  "powers": [
    "ra_additions:stat_bar_example",
    "ra_additions:value_example"
  ],
  "icon": {
    "item": "minecraft:diamond"
  },
  "name": "Magic User",
  "description": "You can harness mana to use in a staff!"
}
```
This example choice adds with a `minecraft:diamond` as its icon.
