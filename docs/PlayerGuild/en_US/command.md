## 权限

##### 本插件默认无需配置任何权限,服主开箱即用

##### 很多下面涉及都类型不知道的 低版本请使用tab提醒,1.12以上会自动提醒

|            权限             |           用途            |  默认拥有者  |  
|:-------------------------:|:-----------------------:|:-------:|
|    playerguild.reload     |          重载插件           |   op    |  
|    playerguild.create     |          创建公会           |  true   |
|    playerguild.addLogo    |       添加logo商城物品        |   op    |
|    playerguild.addShop    |        添加公会商城物品         |   op    |
|  playerguild.setLocation  |         设置pvp场地         |   op    |
|     playerguild.view      |        管理员进行查看信息        |   op    |
|     playerguild.spawn     |         回去公会主城          |  true   |
|   playerguild.setspawn    |         设置公会主城          |  true   |
|  playerguild.createworld  |         创建公会世界          |   op    |
|      playerguild.up       |          升级公会           |  true   |
|     playerguild.leave     |          离开公会           |  true   |
|    playerguild.accept     |         同意加入公会          |  true   |
|     playerguild.deny      |         拒绝加入公会          |  true   |
|     playerguild.open      |         打开公会列表          |  true   |
|   playerguild.acceptPvp   |         同意加入公会战         |  true   |
|    playerguild.denyPvp    |         绝加入公会战          |  true   |
| playerguild.editGuildName |         修改公会名称          |  true   |
|     playerguild.give      |      增加贡献(1.0.2+)       |   op    |
|     playerguild.take      |      减少贡献(1.0.2+)       |   op    |
|      playerguild.set      |      设置贡献(1.0.2+)       |   op    |
|    playerguild.refresh    |       刷新(1.0.3+)        |   op    |
|   playerguild.dissolve    |       刷新(1.2.0+)        |   op    |
| playerguild.create.color  |   公会名可使用颜色代码(1.2.0+)    |   op    |
|    playerguild.signin     |    使用指令后台签到(1.2.7+)     |   op    |
|     playerguild.look      | 使用指令查看当前是否开启公会战(1.2.7+) |   op    |
|     playerguild.start     |  使用指令立即开启赛季公会战(1.3.2+)  |   op    |
|    playerguild.convert    |      转换数据源(1.3.3+)      |   op    |

## 指令:

|                 指令                 |                 用途                  |
|:----------------------------------:|:-----------------------------------:|
|            /plg reload             |               重载配置文件                |
|         /plg create [公会名称]         |                创建公会                 |
|             /plg open              |               打开公会界面                |
|          /plg view  [类型]           |              管理员进行查看信息              |
| /plg setLocation [类型] [场地名] [出生点名] | 设置公会战场地(类型: season:赛季场地, mate:匹配场地) |
|   /plg addShop  [价格] (等级) (限购次数)   |             手持物品上架公会商城              |
|      /plg addLogo  [价格] (等级)       |           手持物品上架公会logo商城            |
|        /plg restore  [玩家名]         |        救命指令,获取玩家公会战开始前备份的装备         |
|      /plg give  [类型] [名称][数量]      |            增加贡献(1.0.2+)             |
|      /plg take  [类型] [名称][数量]      |            减少贡献(1.0.2+)             |
|      /plg set  [类型] [名称][数量]       |            设置贡献(1.0.2+)             |
|            /plg refresh            |      刷新，用于修复公会没任务或者没称号(1.0.3+)      |
|        /plg dissolve  [公会名]        |           强制解散公会(1.2.0+)            |
|       /plg setEquipment (类型)       |          设置公平pvp装备(1.2.0+)          |
|  /plg signin [vault或point] [玩家名]   |         使用指令给玩家后台签到(1.2.7+)         |
|             /plg look              |       使用指令查看当前是否开启公会战(1.2.7+)       |
|             /plg start             |        使用指令立即开启赛季公会战(1.3.2+)        |
|     /plg convert[MySQL-SQLite]     |            转换数据源(1.3.3+)            |
[] 必填 () 非必填

## 特别说明

view 参数说明
```
/plg view location 管理场地
/plg view shop 管理商城
/plg view logo 管理logo
/plg view equipment 管理装备(1.2.0+)
```


give take set 参数说明
```
[类型] 可填三种 guildMoney guildActive player （分别对应公会贡献，公会活跃，玩家贡献）
[名称] 公会的填公会名，玩家类型填玩家名 可用变量(取操作人) ${player} ${guildName}
[数量] 要设置的数量
1. 增加玩家贡献 100
/plg give player [玩家名] 100
2. 使用变量增加公会贡献 100
/plg give guildMoney ${guildName} 100
3. 使用公会名增加公会活跃 100
/plg give guildActive [公会名] 100
```

/plg restore指令 参数说明
```
/plg restore [玩家名] 指令一般无需使用也无需关心  
但是在开启公平公会战后,服务器如果意外崩溃或不可预知原因  
导致玩家背包清空的情况下,就能救服主一命了   
可以指令获取玩家开始公会战时候备份物品到你的背包(记得先清空你背包),然后你还给玩家即可
```

/plg refresh 说明
```
在创建公会后没有生成公会称号或者公会任务
或者 之前没配置称号和任务，现在配置了也可以使用这个指令给公会刷新出来新任务新称号
如果误操作把公会称号在plt里删除掉了，该指令也把被删除的公会称号还原回来
注意，称号是必定根据最新配置刷新，任务的话只会给没有任务的公会进行新增，有旧任务的不做处理
```