# Equipped Trinket

Checks all the players trinket slots with an [Item Condition](https://origins.readthedocs.io/en/latest/types/item_condition_types/).

Type ID: `ra_additions:equipped_trinket`

### Fields

   Field   | Type | Default | Description
-----------|------|---------|-------------
`item_condition` | [Item Condition](https://origins.readthedocs.io/en/latest/types/item_condition_types/) | | The items that are searched for in the trinket slots.

### Example
```json
"condition": {
  	"type": "ra_additions:equipped_trinket",
    "item_condition": {
        "type": "apoli:ingredient",
        "ingredient": {
            "item": "example:nightvision_goggles"
        }
    }
}
```
Returns true if the player has the kunzite trinket equipped.
