# bedrock dev conventions
Some conventions for writing readable and less likely to break Bedrock code

### don't use caps to name anything 
They break stuff!
### use snake casing everywhere (file names, item names, entity names, etc.)
Ex: my_item, snake_casing
### namespace like "my_behaviors:some_item" for items and entities to avoid conflicts with the default packs or other custom packs
### name files with the type of file they are 
Ex: boat.geo.json, boat.entity.json, boat.anim.json (animation), boat.anim_ctrl.json (animation controller)

### Naming tags or scoreboard objectives based on in game entities or items:
-use the actual item name but all lowercase and replace spaces with underscores

For example, consider bone meal in Bedrock:
https://minecraft.gamepedia.com/Bone_Meal#Data_values

Name	    Namespaced ID	Numeric ID             Translation key
Bone Meal   dye	                351                    item.dye.white.name
If you wanted to do something with the scoreboard if there's bone meal on the ground, write something like:
execute @e[type=item,name="Bone Meal"] ~ ~ ~ scoreboard players add @s bone_meal 1

Using the item name but lowercase and underscores for spaces is clearer to read in one command than using Namespaced ID, Numeric ID or Translation Key
