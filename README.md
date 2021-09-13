# ChaosMaven
## Chaos Awakens
Chaos Awakens is a remaster of both the very iconic mod [OreSpawn](https://www.orespawn.com/download.html) and [SoulsOfTheFallen's Chaos Awakens mod pack](https://web.archive.org/web/20180314164908/http://www.dangerzonegame.net/mods.html), built from the ground up. The branch for the 1.16.5 version for Minecraft Forge is located at the [Chaos Awakens Github](https://github.com/ChaosAwakens/ChaosAwakens).

## Usage
#### Make sure to NOT select the dependencies and respository that are inside the buildscript.
To use this maven you should put this code into the repository section of your build.gradle

    maven {
        name = "CurseForge"
        url = "https://www.cursemaven.com"
    }
	maven {
        name = "ChaosMaven"
        url = "https://raw.github.com/ChaosAwakens/ChaosMaven/main"
    }
You must also add this code to the dependencies section of your build.gradle and update the Chaos Awakens and the Geckolib versions to the latest for the current version of Minecraft that Chaos Awakens is updated too.

	implementation fg.deobf("io.github:ChaosAwakens:1.16.5-0.9.0.0-preview")
    implementation fg.deobf('software.bernie.geckolib:geckolib-forge-1.16.5:3.0.35')
