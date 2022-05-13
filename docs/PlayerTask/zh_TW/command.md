## 權限
##### 本插件默認無需配置任何權限,服主開箱即用
##### 很多下面涉及都類型不知道的 低版本請使用tab提醒,1.12以上會自動提醒

| 權限                         | 用途                                      | 默認擁有者           |
|----------------------------|-----------------------------------------|-----------------|
| playertask.addList         | 新增任務                                    | op              |
| playertask.addDemand       | 新增任務目標                                  | op              |
| playertask.addReward       | 新增任務獎勵                                  | op              |
| playertask.addShop         | 新增任務幣商城物品                               | op              |
| playertask.open            | 每日任務gui                                 | op              |
| playertask.shop            | 任務幣商城gui                                | op              |
| playertask.create          | 創建任務                                    | op              |
| playertask.delete          | 刪除任務                                    | op              |
| playertask.view            | 管理任務                                    | op              |
| playertask.vip             | vio權限                                   | op              |
| playertask.getToday        | 立即獲取今日任務                                | op              |
| playertask.delToday        | 清空今日任務列表和全部玩家的任務(1.4.1+)                | op              |
| playertask.delShop         | 刪除對應id的任務幣商城物品                          | op              |
| playertask.getip           | 獲取ip                                    | op              |
| playertask.reload          | 重載配置                                    | op              |
| playertask.edit            | 編輯任務(1.7.1+)                            | op              |
| playertask addNpcTask      | 添加npc任務(1.6.0+)                         | op              |
| playertask delNpcTask      | 刪除npc任務(1.6.0+)                         | op              |
| playertask.setRarity       | 編輯任務稀有度(1.8.7+）                         | op              |
| playertask.changeItem      | 生成任務卷軸 (1.9.0+)                         | op              |
| playertask.setDescription  | 添加任務描述(1.9.7+)                          | op              |
| playertask.coin            | 操作玩家任務幣(1.13.2+)                        | op              |


## 指令(管理員):
| 指令                                                              | 用途                                                                 |
|-----------------------------------------------------------------|--------------------------------------------------------------------|
| /plk addDemand [目標類型] [數量]                                      | 添加任務目標(需要主手持有對應物品)                                                 |
| /plk addReward [獎勵類型] [數量]                                      | 添加任務獎勵(如果獎勵類型是物品需要主手持有對應物品)                                        |
| /plk addShop [類型] [價格]                                          | 添加任務幣商城物品獎勵(類型:限購一次:once;無限購買:infinite)                            |
| /plk create [任務名稱] (任務類型) (任務稀有度)                               | 使用gui來創建任務(推薦)                                                     |
| /plk addList [任務名稱] [稱號目標id] [任務獎勵id]                           | 使用指令方式添加一個任務                                                       |
| /plk delete [類型] [對應id]                                         | 使用指令方式刪除任務,任務目標,任務獎勵                                               |
| /plk view [類型]                                                  | 使用gui裏查看和管理 類型,[list:任務,demand:任務目標,reward:任務獎勵,例如: /plk view list |
| /plk getToday                                                   | 立即執行一次獲取今日任務程序                                                     |
| /plk delToday                                                   | 清空今日任務列表和全部玩家的任務(1.4.1+)                                           |
| /plk delShop [對應ID]                                             | 刪除對應id的任務幣商城物品                                                     |
| /plk getIp                                                      | 獲取ip                                                               |
| /plk reload                                                     | 重載配置                                                               |
| /plk edit [任務id]                                                | 使用gui編輯任務(1.7.1+)                                                  |
| /plk addNpcTask [任務id] [npcId] [是否永久任務] [可完成次數] [冷卻時間] (前置任務id) | 添加npc任務(1.6.0+)                                                    |
| /plk delNpcTask [npcId]                                         | 刪除npc任務(1.6.0+)                                                    |
| /plk setRarity [任務id] [稀有度]                                     | 編輯任務稀有度（1.8.7+）                                                    |
| /plk changeItem [任務id] (玩家名稱)                                   | 生成任務卷軸(1.9.0+)                                                     |
| /plk setDescription [任務id] [任務描述]                               | 添加任務描述(1.9.7+)                                                     |
| /plk coin [類型] [玩家名] [數量]                                       | 操作玩家任務幣數量(1.13.2)                                                  |

## 指令(玩家):
|  指令 | 用途  |
| ------------ | ------------    |
| /plk open    | 打開每日任務gui  |
| /plk shop    | 打開任務幣商城gui  |

```
# 玩家執行指令,中間的0代表按照玩家身份執行,如果玩家沒權限會執行失敗
/plk addReward command 0 eco#give#${player}#666
# 玩家執行指令,中間的1代表按照op身份執行
/plk addReward command 1 eco#give#${player}#666
```

> 任務類型分為 everyday(每日任務)  npc(NPC任務) 不互通