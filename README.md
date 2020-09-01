# bedrock dev conventions
* don't use caps to name anything (they don't work in certain cases)
* use snake casing everywhere (file names, item names, entity names, etc.)...even if the game doesn't use underscores. For example, "appleenchanted" is an item in the game, but in your code refer to it as apple_enchanted as much as possible (ex: adding a scoreboard objective apple_enchanted)
* namespace like "my_behaviors:some_item" for items and entities to avoid conflicts with the default packs or other custom packs
* name files with the type of file they are like - boat.geo.json, boat.anim.json, boat.ctrl.json (animation controller)
