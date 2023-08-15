# Custom Model Render
[Power Types](../power_types.md)

Allows a GeckoLib model to be rendered on the player.

Type ID: `ra_additions:custom_model_render`
### Fields
 | Field | Type | Default | Description | 
|---|---|---|---|
 | `model_location` | [Identifier](../data_types/identifier.md) | _optional_ | The model location to use for the power. | 
 | `slots` | [Array](../data_types/array.md) of [Display Model Type](../data_types/display_model_type.md) | _optional_ | An array of slots used to determine which areas the model should render on. | 

### Example
```json
{
  "type": "ra_additions:custom_model_render",
  "model_path": "ra_additions:test_model",
  "slots": [
    "head",
    "chest",
    "legs",
    "feet"
  ]
}
```

