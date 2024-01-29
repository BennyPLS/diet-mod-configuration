# Survival Diet Mod Configuration

## Description

This project contains the configuration for the Diet Mod. The Diet Mod is a modification for Minecraft
that allows players to manage their character's diet for a more immersive gameplay experience.

This configuration diverges from the default configuration in the following ways:

* Add de-buffs for ignoring your character's diet.
* Sets a default level for the food groups.

## Installation

1. Download the Diet Mod Configuration files.
2. Download the Diet Mod.
3. Open the .jar file for the Diet Mod (Winrar/7zip).
4. Replace the folder contents of `data/diet/diet` folder for the `diet` folder contents.
5. Save the .jar file.
6. Run Minecraft.
7. Replace in the .minecraft folder the contents of `config/diet-server.toml` for the contents of the `diet-server.toml`
   file inside config folder.
8. Restart Minecraft.
9. Enjoy!

## In Depth information

This section contains in depth information about the Configuration.
This configuration is highly customizable, you can change the values of the food groups, the de-buffs and the buffs.

### Food Groups

The Diet Mod divides food into five food groups, the default levels for each food group are:

* Fruits - 0.35f - 35%
* Vegetables - 0.35f - 35%
* Grains - 0.35f - 35%
* Proteins - 0.35f - 35%
* Sugars - 0.15f - 15%

**Note**: Death will reset the food groups to their default levels.

## De-Buffs

1. **Malnourishment**
    - Effects:
        - Reduces max health by 50%.
        - Reduces movement speed by 20%.
        - Reduces attack damage by 2.0.
        - Reduces attack speed by 20%.
        - Reduces armor by 20%.
        - Reduces armor toughness by 20%.
        - Gives the player nausea with power 1.
    - Condition:
        - Groups: Fruits, Vegetables, Proteins, Grains
        - Threshold:
            - Below: 5%

2. **Movement Speed Reduction**
    - Effect: Reduces the player's base movement speed by 25%.
    - Condition:
        - Groups: Fruits, Vegetables
        - Threshold:
            - Below: 30%

3. **Attack Damage and Speed Reduction**
    - Effects:
        - Reduces the player's attack damage by 10% and reduces by 1.0.
        - Reduces the player's attack speed by 10%.
    - Condition:
        - Groups: Proteins, Grains
        - Threshold:
            - Below: 30%

4. **Mining Fatigue**
    - Effect: Gives the player mining fatigue with power 2.
    - Condition:
        - Groups: Grains
        - Threshold:
            - Below: 30%

5. **Max Health Reduction**
    - Effect: Reduces the player's max health by 10%.
    - Condition:
        - Groups: Fruits, Vegetables, Proteins, Grains
        - Threshold:
            - Below: 30%
        - Groups: Sugars
        - Threshold:
            - Below: 10%

## Buffs

1. **Max Health, Attack Damage and Speed Increase**
    - Effects:
        - Increases the player's max health by 2.0.
        - Increases the player's attack damage by 10% and increases by 2.0.
        - Increases the player's attack speed by 10%.
    - Condition:
        - Groups: Proteins, Grains
        - Threshold:
            - Above: 80%
            - Below: 100%

2. **Max Health and Armor Toughness Increase**
    - Effects:
        - Increases the player's max health by 2.5.
        - Increases the player's armor toughness by 1.0.
    - Condition:
        - Groups: Proteins, Fruits, Vegetables, Grains
        - Threshold:
            - Above: 75%
            - Below: 100%

3. **Movement Speed Increase and Hunger**
    - Effects:
        - Increases the player's movement speed by 30%.
        - Gives the player hunger with power 4.
    - Condition:
        - Groups: Sugars
        - Threshold:
            - Above: 80%
            - Below: 100%

## Credits

This project uses the following open source projects:

* [Diet Mod](https://www.curseforge.com/minecraft/mc-mods/diet)
  by [The_Wabbit](https://www.curseforge.com/members/the_wabbit)