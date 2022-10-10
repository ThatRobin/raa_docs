# Power Active

Checks whether the entity has a power that uses the specified [Power Type](https://origins.readthedocs.io/en/latest/types/power_types/), excluding those in the blacklist, and is "active", meaning that the entity has the power and the power has all its conditions fulfilled.

Type ID: `ra_additions:active_power_type`


### Fields

Field  | Type | Default | Description
-------|------|---------|-------------
`power_type` | [Identifier](../data_types/identifier.md) | | The namespaced ID of the power type which will be checked to see if any are active.
`blacklisted_powers` | [Array](../data_types/array.md) of [Identifiers](../data_types/identifier.md) | | The namespaced IDs of powers that will be excluded from the check.


### Examples
```json
"condition": {
  	"type": "ra_additions:active_power_type",
      "power_type": "apoli:elytra_flight",
      "blacklisted_powers": [
          "example:elytra_power"
      ]
}
```
This will return true if the player has any elytra flight power that isn't "example:elytra_power".
