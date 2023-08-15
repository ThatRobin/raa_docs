# Tag Extensions
RAA has extended tag functionality into Powers and Actions.

You can now store your actions, or powers, into tags, and use them with the `/raa` command.

Power Tags can also be used in conjunction with Origins, and also RAA Choices. If you have origins installed, you can make a power tag with the same id as an origin/choice, and the powers specified will be added to the origin/choice, without the need to edit that origin/choice's datapack.
### Examples
```json
{
  "replace": false,
  "values": [
    "ra_additions:condition_example_2"
  ]
}
```
This example creates a tag out of the `ra_additions:condition_example_2` power, stored at `ra_additions:powers/condition_example_2.json`, and will add the listed powers to the choice `ra_additions:choice_example`
```json
{
  "replace": false,
  "values": [
    "ra_additions:action_example_1"
  ]
}
```
This example creates a tag out of the `ra_additions:action_example_1` entity action, stored at `ra_additions:actions/entity/action_example_1.json`
