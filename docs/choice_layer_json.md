# Layer JSON Format
This is the format of a JSON file describing a layer. Layers are collections of choices, and a player can have a single choice on each layer.

Layer files need to be placed inside the `choice_layers` folder within your namespace.

 | Fields | Type | Default | Description | 
|---|---|---|---|
 | `choices` | [Array](data_types/array.md) of [Identifiers](data_types/identifier.md) |   | Defines the choices that should be in this layer. | 
 | `enabled` | [Boolean](data_types/boolean.md) | `true` | If set to false, this layer will be unavailable. | 

### Examples
```json
{
  "choices": [
    "ra_additions:choice_example"
  ]
}
```
This example choice layer allows you to choose an example choice.
