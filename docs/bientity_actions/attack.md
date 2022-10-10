### Attack

The actor entity will damage the target enemy as if they had just been hit with the weapon in the actors hand.

Type ID: `ra_additions:attack`

### Fields

Field  | Type | Default | Description
-------|------|---------|-------------
`allow_enchants` | [Boolean](../data_types/boolean.md) | `false` | Will the damage take weapon enchants into account.
`allow_weapons` | [Boolean](../data_types/boolean.md) | `false` | Will the damage take weapon damage into account.
`allow_effects` | [Boolean](../data_types/boolean.md) | `false` | Will the damage take status effects into account
`allow_attributes` | [Boolean](../data_types/boolean.md) | `false` | Will the damage take the strength attribute into account.
`source` | [Damage Source](../data_types/damage_source.md) | | The damage source to be used. Controls e.g. the death message, invulnerabilities (e.g. towards fire), or whether armor is taken into account.


### Examples

```json
"bientity_action": {
    "type": "ra_additions:attack",
    "allow_enchants": true,
    "allow_weapons": true,
    "allow_effects": true,
    "allow_attributes": true,
    "source": {
        "name": "player",
        "bypasses_armor": true
    }
}
```

This example will deal damage to the target as if the actor has hit them, the damage is calculated by the actor's weapon, enchants, status effects and additional attributes.