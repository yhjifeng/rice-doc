## Permissions
##### This plug-in default does not need to configure any permissions, the owner of the service out of the box that use
##### a lot of the following types involved do not know the low version, please use the tab reminder, 1.12 or more will automatically remind
| Permissions                         | Usage                                 | Default owner |
|-------------------------------------|---------------------------------------|---------------|
| playerintensify.reload              | reload plugin                         | op            |
| playerintensify.getip               | Get ip                                | op            |
| playerintensify.giveryancokes       | get hearthstone carbon                | op            |
| playerintensify.giveenchantedcokes  | getadvancedcarbon                     | op            |
| playerintensify.giveprotectioncard  | get fortifiedcokes                    | op            |
| playerintensify.giveprotectioncard  | get fortifiedcokes                    | op            |
| playerintensify.probability         | test the probability of reinforcement | op            |
| playerintensify.createhd            | Create a reinforcement hologram       | op            |
| playerintensify.givesecretmedicines | Get the reinforcement secret          | op            |
| playerintensify.up                  | Level up                              | op            |
| playerintensify.adminUp             | Force level up                        | op            |
| playerintensify.adminUp             | Force level up                        | op            |
| playerintensify.adminUp             | Force level up                        | op            |
| playerintensify.giveIntensifyCard   | Get a fortification voucher           | op            |

## Command:
| Command                                             | Usage                                                                  |
|-----------------------------------------------------|------------------------------------------------------------------------|
| /plis reload                                        | Reload the plugin                                                      |
| /plis giveRyanCokes [number]                        | Give the player a specified number of enhanced stones                  |
| /plis giveEnchantedCokes [quantity]                 | Give the player a specified number of Advanced Enhanced Cokes          |
| plis giveProtectionCokes [quantity]                 | Give the player a specified number of Advanced Enhanced Cokes          |
| /plis giveProtectionCard [quantity]                 | Give the player a specified number of Enhanced Protection Certificates |
| /plis probability [level]                           | Test the current level's enhancement rate                              |
| /plis createHd                                      | Create a hologram ranking                                              |
| /plis giveSecretMedicines [number]                  | Get Secret Medicines                                                   |
| /plis up                                            | Raise the enhancement level                                            |
| /plis adminUp                                       | Administer the setting of enhancement levels                           |
| /plis giveIntensifyCard [Type] [Level] [Quantity]   | Get Intensify Vouchers                                                 |

#### Intensify Card Type
```
# IntensifyCard type -> default probability e.g. iron_ingot probability is 1 percent
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
    gold_ingot: "&5 gold equipment enhancement coupons"
    platinum: "&5 platinum equipment enhancement coupons"
    emerald: "&5 Emerald coupons"
    diamond: "&5 diamond equipment coupon"
    intensify_card: "&5 equipment enhancement coupons"
```