
![Skinify Logo](https://raw.githubusercontent.com/Dorcupi/skinify/main/skinifyplayermods.png)


# Skinify

When you decide that being a player is too boring, and you need to be a spider, snowman, or minature instead.

## About

Skinify is not necessarly a resource pack but a template that allows you to make an resource pack with new versions of your favorite skins. (more info later) These new versions can then be used for a variety of ways.


## Installation

The creation/installation process is quite complicated but once you read the steps, it becomes quite simple.

1. Download the template you want. As of writing this (July 2nd, 2023), there are 3 templates, SnowSteves, MiniCraft, and SpideySteves.

2. Extract the zip and choose which folder you will be using depending on if your skin is a Normal (steve) or a Slim. (alex)

3. Copy all the contents in the folder and paste it into the Template Pack folder. Then move it into the folder path specified below.

```
assets\minecraft\models\custom\
```

4. Get the Minecraft skin you will be using and copy and paste it into the Template Pack folder. Then move it to the folder path specified below.

```
assets\minecraft\textures\custom\
```

5. Delete the placeholder skin. Then remane your skin to whatever you like but make sure you know the name. Then go to the folder path **assets\minecraft\models\custom** and open one of the json files

6. Edit the file so that in the **textures** area, both the places that say skin is the name your skin. Make sure you don't include the **.png**. Here is an example.

```
"textures": {
		"0": "minecraft:custom/(skin name goes here)",
		"particle": "minecraft:custom/(skin name goes here)"
	},
```

7. Repeat steps 6-7 for any additional files if there is any.

8. Then head to the folder path **assets\minecraft\models\item** and open **flint.json**. Copy all the **custom_model_data** numbers and keep them for later. Also make sure that all the **model** sections link up to models in the folder path **assets\minecraft\models\custom**. Not all template packs will have two but some do. Here is an example.

```
"overrides":
[
			{ "predicate": { "custom_model_data": (copy number here)}, "model" : (make sure these link)},
]

```

9. If you want multiple skins then you need to redo all those steps in the same template pack. Make sure all files have a different name. Make sure that the **flint.json** file from the last step is updated to support all the skins. There needs to be commas at the ends of all curly brackets except the last one. Here is a example.

```
"overrides":
[
			{ "predicate": { "custom_model_data": (unique number)}, "model" : (unique name)},
            { "predicate": { "custom_model_data": (unique number)}, "model" : (unique name)}
]

```

10. Now you can copy the template pack and paste it into your resource pack folder. The resource pack is finished! You can now launch the game. If you did everything correctly, you should now be able to modify the following command with your custom model data number and get the model you wanted.

```
/give @s flint{CustomModelData:(custom model data number)}
```
## Ideas for Use

- Make a custom entity by summoming a mob that's invisible with the item on its head

- Make a display by placing a invisible item frame and putting the item inside

- Make a custom build and incorporate it inside the build

## Screenshots

![MiniSteves 1](https://raw.githubusercontent.com/Dorcupi/skinify/main/screenshots/miniSit2.png)

![SnowSteves 1](https://raw.githubusercontent.com/Dorcupi/skinify/main/screenshots/snowman1.png)

![MiniSteves 2](https://raw.githubusercontent.com/Dorcupi/skinify/main/screenshots/miniSit5.png)

![SpideySteves 1](https://raw.githubusercontent.com/Dorcupi/skinify/main/screenshots/spidey1.png)

![SnowSteves 2](https://raw.githubusercontent.com/Dorcupi/skinify/main/screenshots/snowman2.png)

![SpideySteves 2](https://raw.githubusercontent.com/Dorcupi/skinify/main/screenshots/spidey3.png)


## About Me
I'm Dorcupi, a Minecraft datapack developer, Python developer, YouTuber, and 100% hobbyist. I enjoy coding and I hope you enjoy what I make.


## License

[Skinify](https://github.com/Dorcupi/skinify) © 2023 by [Dorcupi](https://github.com/Dorcupi) is licensed under [Attribution-NoDerivatives 4.0 International](https://creativecommons.org/licenses/by-nd/4.0/?ref=chooser-v1)