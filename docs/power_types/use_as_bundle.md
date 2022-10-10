# Use as Bundle

[Power Type](../power_types.md).

Allows an item to be used like a bundle, with a customizable capacity.

Type ID: `ra_additions:use_as_bundle`

### Fields

Field  | Type | Default | Description
-------|------|---------|-------------
`hold_amount` | [Integer](../data_types/integer.md) | `64` | the amount of items you can store in the bundle.
`item_condition` | [Item Condition Type](https://origins.readthedocs.io/en/latest/types/item_condition_types/) | _optional_ | Items that fulfil this condition, will be bundle-like.


### Example
```json
{
	"type": "ra_additions:use_as_bundle",
	"hold_amount": 64,
	"item_condition": {
		"type": "apoli:nbt",
		"nbt": "{isBundle:1b}"
	}
}
```
