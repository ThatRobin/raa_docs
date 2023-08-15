# Condition JSON Format
This is the format of a JSON file describing a condition. These can be used in place of creating an condition inside of a power. 

Condition JSON files need to be placed inside the `data/<namespace>/{Condition Type}` folder of your datapack. Where the `{Condition Type}` is either `entity`, `bientity`, `block` or `item`.
### Examples
```json
{
  "type": "apoli:sneaking"
}
```
This example is a condition that checks if the player is sneaking.
```json
{
  "type": "apoli:active_self",
  "entity_action": {
    "type": "apoli:add_velocity",
    "y": 2
  },
  "condition": {
    "type": "ra_additions:evaluate_condition",
    "entity_condition": "ra_additions:condition_example_1"
  },
  "cooldown": 20,
  "hud_render": {
    "should_render": false
  },
  "key": {
    "key": "key.ra_additions.keybind_example"
  }
}
```
This is an example of one way that you can use an entity condition from a file
