## 权限

##### 本插件默认无需配置任何权限,服主开箱即用

##### 很多下面涉及都类型不知道的 低版本请使用tab提醒,1.12以上会自动提醒

| 权限                                       | 用途          | 默认拥有者         |
|------------------------------------------|-------------|---------------|
| playerintensify.reload                   | 重载插件        | op            |
| playerintensify.giveryancokes            | 获取炉岩碳       | op            |
| playerintensify.giveenchantedcokes       | 获取高级炉岩碳     | op            |
| playerintensify.giveprotectioncard       | 获取qianghua保护券     | op            |
| playerintensify.probability              | 测试qianghua概率      | op            |
| playerintensify.createhd                 | 创建qianghua排行全息图   | op            |
| playerintensify.givesecretmedicines      | 获取qianghua秘药      | op            |
| playerintensify.up                       | 提升qianghua等级      | op            |
| playerintensify.adminUp                  | 强行设置qianghua等级    | op            |
| playerintensify.giveIntensifyCard        | 获取qianghua券       | op            |

## 指令:

| 指令                                      | 用途                              |
|-----------------------------------------|---------------------------------|
| /plis reload                            | 重载插件                            |
| /plis giveRyanCokes [数量]                | 给对应玩家数量的炉岩碳                     |
| /plis giveEnchantedCokes [数量]           | 给对应玩家数量的高级炉岩碳                   |
| /plis giveProtectionCard [数量]           | 给对应玩家数量的qianghua保护券                   |
| /plis probability  [等级]                 | 测试当前qianghua概率                        |
| /plis createHd                          | 创建全息图qianghua排行(需HolographicDisplays) |
| /plis giveSecretMedicines [数量]          | 获取qianghua秘药                          |
| /plis up                                | 提升qianghua等级                          |
| /plis adminUp                           | 强行设置qianghua等级                        |
| /plis giveIntensifyCard [类型] [等级] [数量]  | 获取qianghua券                           |

#### qianghua券类型

```
# qianghua券类型  -> 默认概率 例如 iron_ingot 概率为百分之1
# iron_ingot -> 1
# bronze -> 5
# bai_yin -> 10
# gold_ingot -> 30
# platinum -> 50
# emerald -> 70
# diamond -> 90
# intensify_card -> 100
intensifyCardType:
    iron_ingot: "&5黑铁装备qianghua券"
    bronze: "&5青铜装备qianghua券"
    bai_yin: "&5白银装备qianghua券"
    gold_ingot: "&5黄金装备qianghua券"
    platinum: "&5铂金装备qianghua券"
    emerald: "&5翡翠装备qianghua券"
    diamond: "&5钻石装备qianghua券"
    intensify_card: "&5装备qianghua券"
```