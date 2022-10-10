### Open Choice Screen

Opens the choice screen for the player, allowing for them to select a specific choice.

Type ID: `ra_additions:open_choice_screen`

### Fields

Field  | Type | Default | Description
-------|------|---------|-------------
`choice_layer` | [Identifier](../data_types/identifier.md) | | ID of the choice layer that the action will open.

### Example
```json
{
    "entity_action": {
        "type": "ra_additions:open_choice_screen",
        "choice_layer": "example:choice"
    }
}
```

This example will open the `example:choice` (`data/example/choice_layers/choice.json`) choice layer for the player.
