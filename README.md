# Forge Crater (Fabric, Minecraft 1.21.11)

Right-click with the **Forge Shard** (aim at the ground). It charges with cyan soul fire,
detonates, carves a crater (radius 24), lines it with dark/cyan crust and sends veins across the terrain.

Get the item: `/give @s forge_crater:forge_shard` (or craft: amethyst/diamond ring around a nether star).

Tweak in `CraterManager.RADIUS`, `ForgeShardItem.COOLDOWN_TICKS`, `CraterEvent.CHARGE_TICKS/CARVE_TICKS`.

Build: add a Gradle wrapper (`gradle wrapper` or copy one from the official template at fabricmc.net/develop/template), then `./gradlew build`. Jar ends up in build/libs/.

## Getting the .jar without installing anything
1. Create a new GitHub repo and upload everything in this folder (including the `.github` folder).
2. Open the repo's **Actions** tab -> "Build jar" -> wait for the green check.
3. Open the finished run and download the **forge-crater-jar** artifact (a zip containing `forge-crater-1.0.0.jar`).
4. Drop that jar into your `mods` folder along with Fabric API 0.141.1+1.21.11.
