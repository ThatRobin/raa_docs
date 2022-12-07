### Execute Action

Executes a given action from an action file.

Type ID: `ra_additions:execute_action`

### Fields:

Field  | Type | Default | Description
-------|------|---------|-------------
`{Action Type}_action` | [Identifier]((../data_types/identifier.md) |  |  The ID of an action, where `{Action Type}` matches the action that is being executed.

### Example

```json
"entity_action": {
    "type": "ra_additions:execute_action",
    "entity_action": "origins:entity_test"
}
```
This example will execute an entity action from `origins/actions/entity/entity_test.json`.