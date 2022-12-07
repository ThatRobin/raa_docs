# Action JSON Format

This is the format of a JSON file describing an action. These can be used in place of creating an action inside of an origin. 

Action JSON files need to be placed inside the `data/<namespace>/{Action Type}` folder of your datapack. Where the `{Action Type}` is either `entity`, `bientity`, `block` or `item`.

### Examples

```json
{
    "type": "origins:add_velocity",
    "y": 2
}
```

This example is an action that launches the player into the air.