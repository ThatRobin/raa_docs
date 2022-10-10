### Universal Powers

Custom Content Packs allow you to use the same power system as Origins (Apoli), with your custom content for greater variety. In order to use the universal power system. you make your power files as you would in Origins. And then make the directories `/data/<namespace>/universal_powers/` and create a JSON file in there (it can be named anything)
Then, in this file, you enter your powers, and entities.

Fields  | Type | Default | Description
--------|------|---------|-------------
`powers` | [Array](data_types/array.md) of [Identifiers](data_types/identifier.md) | _optional_ | The namespace and IDs of the powers you want to give to all entities.
`entity_entry` | [Object](data_types/object.md) | _optional_ | An object that accepts either an `entity` or a `tag` [Identifier](data_types/identifier.md). Cannot be both.

### Examples
```json
{
	"powers": [
		"namespace:power_name",
		"namespace:power_name_2"
	],
	"entity_entry": {
		"entity": "minecraft:player"
	}
}
```
This example would apply the powers `namespace:power_name` and `namespace:power_name_2` to all players.

```json
{
	"powers": [
		"namespace:power_name",
		"namespace:power_name_2"
	],
	"entity_entry": {
		"tag": "minecraft:skeletons"
	}
}
```
This example would apply the powers `namespace:power_name` and `namespace:power_name_2` to all entities in the `minecraft:skeletons` Entity Type tag.
