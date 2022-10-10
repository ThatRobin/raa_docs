# Resource Percentage

[Entity Condition](../entity_conditions.md).

Checks the percentage of a resource.

Type ID: `ra_additions:resource_percentage`

### Fields

Field  | Type | Default | Description
-------|------|---------|-------------
`resource` | [Identifier](../data_types/identifier.md) | | ID of the power type that defines the resource which exists on the player.
`comparison` | [Comparison](https://origins.readthedocs.io/en/latest/types/data_types/comparison/) | `"=="` | How the value of the power that will be evaluated should be compared to the specified value.
`percentage` | [Integer](../data_types/integer.md) | `50` | The percentage value to compare the value of the power that will be evaluated to. `(e.g 50%)`

### Example
```json
"condition": {
    "type": "ra_additions:resource_percentage",
    "stat_bar": "example:resource_power",
    "comparison": ">=",
	"percentage": 50
}
```
This condition checks to see if `example:resource_power` has a value greater than 50% of its total.
