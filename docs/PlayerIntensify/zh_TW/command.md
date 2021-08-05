## 權限
##### 本插件默認無需配置任何權限,服主開箱即用
##### 很多下面涉及都類型不知道的 低版本請使用tab提醒,1.12以上會自動提醒
|  權限 | 用途  | 默認擁有者 |
| ------------ | ------------ | ------------ |
| playerintensify.reload  | 重載插件  | op |
| playerintensify.getip  | 獲取ip  | op |
| playerintensify.giveryancokes  | 獲取爐巖碳  | op |
| playerintensify.giveenchantedcokes  | 獲取高級爐巖碳  | op |
| playerintensify.giveprotectioncard  | 獲取強化保護券  | op |
| playerintensify.probability  | 測試強化概率  | op |
| playerintensify.createhd  | 創建強化排行全息圖  | op |
| playerintensify.givesecretmedicines| 獲取強化秘藥|op|
| playerintensify.up| 提升強化等級|op|
| playerintensify.adminUp| 強行設置強化等級|op|
| playerintensify.giveIntensifyCard| 獲取強化券|op|

## 指令:
|  指令 | 用途  |
| ------------ | ------------ |
|/plis reload                      |      重載插件|
|/plis getIp                         |    獲取服務器ip地址|
|/plis giveRyanCokes [數量]         |     給對應玩家數量的爐巖碳|
|/plis giveEnchantedCokes [數量]  |       給對應玩家數量的高級爐巖碳|
|/plis giveProtectionCard [數量]   |      給對應玩家數量的強化保護券|
|/plis probability  [等級]           |    測試當前強化概率|
|/plis createHd                      |    創建全息圖強化排行(需HolographicDisplays)|
|/plis giveSecretMedicines [數量]   |      獲取強化秘藥|
|/plis up   |      提升強化等級|
|/plis adminUp    |      強行設置強化等級|
|/plis giveIntensifyCard [類型] [等級] [數量]   |      獲取強化券|

#### 強化券類型
```
# 強化券類型  -> 默認概率 例如 iron_ingot 概率為百分之1
# iron_ingot -> 1
# bronze -> 5
# bai_yin -> 10
# gold_ingot -> 30
# platinum -> 50
# emerald -> 70
# diamond -> 90
# intensify_card -> 100
intensifyCardType:
    iron_ingot: "&5黑鐵裝備強化券"
    bronze: "&5青銅裝備強化券"
    bai_yin: "&5白銀裝備強化券"
    gold_ingot: "&5黃金裝備強化券"
    platinum: "&5鉑金裝備強化券"
    emerald: "&5翡翠裝備強化券"
    diamond: "&5鉆石裝備強化券"
    intensify_card: "&5裝備強化券"
```