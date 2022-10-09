## Permissions

##### This plugin does not require any permissions to be configured by default, the service owner can use it out of the box

##### Many of the following types are not known. Please use the tab to remind you of low versions, 1.12 or above will be automatically reminded.

|             Permissions             |                  Usage                  | Default owner  |
|:-----------------------------------:|:---------------------------------------:|:--------------:|
|       playerIntensify.reload        |              reload plugin              |       op       |
|    playerIntensify.giveRyanCokes    |             getStrongstone              |       op       |
| playerIntensify.giveEnchantedCokes  |          Get advanced fossils           |       op       |
| playerIntensify.giveProtectionCard  |      get Enhanced Protection Cokes      |       op       |
| playerIntensify.giveProtectionCard  |                   op                    |
|      playerIntensify.createHd       | Create a reinforcement ranking hologram |       op       |
| playerIntensify.giveSecretMedicines |  Get a boost to your enhancement rate   |       op       |
|         playerIntensify.up          |    Command to level up enhancements     |       op       |
|       playerIntensify.adminUp       |             Force leveling              |       op       |
|  playerIntensify.giveIntensifyCard  |       Get a reinforcement ticket        |       op       |

## Command:

|                         command                          |                                  use                                   |
|:--------------------------------------------------------:|:----------------------------------------------------------------------:|
|                       /plis reload                       |                             reload plugin                              |
|           /plis giveRyanCokes [number] (name)            |       Give the player a specified number of fortification stones       |
|         /plis giveEnchantedCokes [number] (name)         |     Give the player a specified number of Advanced EnchantedCokes      |
|         /plis giveProtectionCard [number] (name)         | Give the player a specified number of Enhanced Protection Certificates |
|                /plis probability [level]                 |               Test the current level's enhancement rate                |
|                      /plis createHd                      |                       Create a hologram ranking                        |
|        /plis giveSecretMedicines [number] (name)         |              Gets the enhancement probability bonus item               |
|                         /plis up                         |                        Raise enhancement level                         |
|                      /plis adminUp                       |                   Manage setting enhancement levels                    |
| /plis giveIntensifyCard [type] [level] [quantity] (name) |                           Get IntensifyCard                            |

### Intensify Card Type

```
### IntensifyCard type -> e.g. iron_ingot is 1 % probability
# iron_ingot -> 1
# bronze -> 5
# bai_yin -> 10
# gold_ingot -> 30
# platinum -> 50
# emerald -> 70
# diamond -> 90
# intensify_card -> 100
intensifyCardType:
    iron_ingot: "&5 black iron equipment enhancement coupons"
    bronze: "&5 bronze equipment enhancement coupons"
    bai_yin: "&5 silver equipment enhancement coupons"
    gold_ingot: "&5 gold coupons"
    platinum: "&5 platinum coupons"
    emerald: "&5 Emerald coupons"
    diamond: "&5 diamond equipment enhancement coupons"
    intensify_card: "&5 equipment enhancement coupons"
```