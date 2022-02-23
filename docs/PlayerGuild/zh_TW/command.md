## 權限

##### 本插件默認無需配置任何權限,服主開箱即用

##### 很多下面涉及都類型不知道的 低版本請使用tab提醒,1.12以上會自動提醒

| 權限                              | 用途              | 默認擁有者  |
|---------------------------------|--- --------------|--------|
| playerguild.reload              | 重載插件            | op     |
| playerguild.create              | 創建公會            | true   |
| playerguild.addLogo             | 添加logo商城物品      | op     |
| playerguild.addShop             | 添加公會商城物品        | op     |
| playerguild.setLocation         | 設置pvp場地         | op     |
| playerguild.view                | 管理員進行查看信息       | op     |
| playerguild.spawn               | 回去公會主城          | true   |
| playerguild.setspawn            | 設置公會主城          | true   |
| playerguild.createworld         | 創建公會世界          | op     |
| playerguild.up                  | 升級公會            | true   |
| playerguild.leave               | 離開公會            | true   |
| playerguild.accept              | 同意加入公會          | true   |
| playerguild.deny                | 拒絕加入公會          | true   |
| playerguild.open                | 打開公會列表          | true   |
| playerguild.acceptPvp           | 同意加入公會戰         | true   |
| playerguild.denyPvp             | 絕加入公會戰          | true   |
| playerguild.editGuildName       | 修改公會名稱          | true   |
| playerguild.give                | 增加貢獻(1.0.2+)    | op     |
| playerguild.take                | 減少貢獻(1.0.2+)    | op     |
| playerguild.set                 | 設置貢獻(1.0.2+)    | op     |
| playerguild.refresh             | 刷新(1.0.3+)      | op     |
| playerguild.dissolve            | 刷新(1.2.0+)      | op     |
| playerguild.create.color        | 公會名可使用顏色代碼(1.2.0+) | op |
| playerguild.signin              | 使用指令後臺簽到(1.2.7+) | op |
| playerguild.look              | 使用指令查看當前是否開啟公會戰(1.2.7+) | op |

## 指令:

| 指令                                 | 用途                                  |
|------------------------------------|-------------------------------------|
| /plg reload                        | 重載配置文件                              |
| /plg create [公會名稱]                 | 創建公會                                |
| /plg open                          | 打開公會界面                              |
| /plg view  [類型]                    | 管理員進行查看信息                           |
| /plg setLocation [類型] [場地名] [出生點名] | 設置公會戰場地(類型: season:賽季場地, mate:匹配場地) |
| /plg addShop  [價格] (等級) (限購次數)     | 手持物品上架公會商城                          |
| /plg addLogo  [價格] (等級)            | 手持物品上架公會logo商城                      |
| /plg restore  [玩家名]                | 救命指令,獲取玩家公會戰開始前備份的裝備                |
| /plg give  [類型] [名稱][數量]           | 增加貢獻(1.0.2+)                        |
| /plg take  [類型] [名稱][數量]           | 減少貢獻(1.0.2+)                        |
| /plg set  [類型] [名稱][數量]            | 設置貢獻(1.0.2+)                        |
| /plg refresh                       | 刷新，用於修復公會沒任務或者沒稱號(1.0.3+)           |
| /plg dissolve  [公會名]               | 強製解散公會(1.2.0+)                      |
| /plg setEquipment (類型)             | 設置公平pvp裝備(1.2.0+)                   |
| /plg signin [vault或point] [玩家名]    | 使用指令給玩家後臺簽到(1.2.7+)                 |
| /plg look                          | 使用指令查看當前是否開啟公會戰(1.2.7+)             |
[] 必填 () 非必填

## 特別說明

view 參數說明
```
/plg view location 管理場地
/plg view shop 管理商城
/plg view logo 管理logo
/plg view equipment 管理裝備(1.2.0+)
```


give take set 參數說明
```
[類型] 可填三種 guildMoney guildActive player （分別對應公會貢獻，公會活躍，玩家貢獻）
[名稱] 公會的填公會名，玩家類型填玩家名 可用變量(取操作人) ${player} ${guildName}
[數量] 要設置的數量
1. 增加玩家貢獻 100
/plg give player [玩家名] 100
2. 使用變量增加公會貢獻 100
/plg give guildMoney ${guildName} 100
3. 使用公會名增加公會活躍 100
/plg give guildActive [公會名] 100
```

/plg restore指令 參數說明
```
/plg restore [玩家名] 指令一般無需使用也無需關心  
但是在開啟公平公會戰後,服務器如果意外崩潰或不可預知原因  
導致玩家背包清空的情況下,就能救服主一命了   
可以指令獲取玩家開始公會戰時候備份物品到你的背包(記得先清空你背包),然後你還給玩家即可
```

/plg refresh 說明
```
在創建公會後沒有生成公會稱號或者公會任務
或者 之前沒配置稱號和任務，現在配置了也可以使用這個指令給公會刷新出來新任務新稱號
如果誤操作把公會稱號在plt裏刪除掉了，該指令也把被刪除的公會稱號還原回來
註意，稱號是必定根據最新配置刷新，任務的話只會給沒有任務的公會進行新增，有舊任務的不做處理
```