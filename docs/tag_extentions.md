# Tag Extentions

RAA has extended tag functionality into Powers and Actions.

You can now store your actions, or powers, into tags, and use them with the `/raa` command.

Power Tags can also be used in conjunction with Origins, and also RAA Choices. If you have origins installed, you can make a power tag with the same id as an origin/choice, and the powers specified will be added to the origin/choice, without the need to edit that origin/choice's datapack.

### Example

```json
{
    "replace": false,
    "values": [
        "origins:bientity_test"
    ]
}
```
This example creates a tag out of the `origins:bientity_test` bientity action, stored at `origins/actions/bientity/bientity_test.json`