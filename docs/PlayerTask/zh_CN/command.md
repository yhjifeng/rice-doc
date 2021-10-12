## 权限
##### 本插件默认无需配置任何权限,服主开箱即用  
##### 很多下面涉及都类型不知道的 低版本请使用tab提醒,1.12以上会自动提醒

|  权限 | 用途  | 默认拥有者 |
| ------------ | ------------ | ------------ |
| playertask.addList  | 新增任务  | op |
| playertask.addDemand  | 新增任务目标  | op |
| playertask.addReward  | 新增任务奖励  | op |
| playertask.addShop  | 新增任务币商城物品  | op |
| playertask.open  | 每日任务gui  | op |
| playertask.shop  | 任务币商城gui  | op |
| playertask.create  | 创建任务  | op |
| playertask.delete  | 删除任务  | op |
| playertask.view  | 管理任务  | op |
| playertask.vip  | vio权限  | op |
| playertask.getToday  | 立即获取今日任务  | op |
| playertask.delShop  | 删除对应id的任务币商城物品  | op |
| playertask.getip  | 获取ip  | op |
| playertask.reload  | 重载配置  | op |
| playertask.edit  | 编辑任务  | op |
| playertask.setRarity  | 编辑任务稀有度1.8.7+）  | op |

## 指令(管理员):
|  指令 | 用途  |
| ------------ | ------------ |
| /plk addDemand [目标类型] [数量] | 添加任务目标(需要主手持有对应物品)  |
| /plk addReward [奖励类型] [数量] | 添加任务奖励(如果奖励类型是物品需要主手持有对应物品) |
| /plk addShop [类型] [价格] | 添加任务币商城物品奖励(类型:限购一次:once;无限购买:infinite) |
| /plk create [任务名称]   |  使用gui来创建任务(推荐) |
| /plk addList [任务名称] [称号目标id] [任务奖励id] | 使用指令方式添加一个任务 |
| /plk delete [类型] [对应id] | 使用指令方式删除任务,任务目标,任务奖励 |
| /plk view [类型] | 使用gui里查看和管理 类型,[list:任务,demand:任务目标,reward:任务奖励,例如: /plk view list|
| /plk getToday | 立即执行一次获取今日任务程序|
|/plk delShop [对应ID] | 删除对应id的任务币商城物品|
|/plk getIp | 获取ip|
|/plk reload | 重载配置|
|/plk edit [任务id] | 使用gui编辑任务  |
|/plk setRarity [任务id] [稀有度]| 编辑任务稀有度（1.8.7+） ｜

## 指令(玩家):
|  指令 | 用途  |
| ------------ | ------------    |
| /plk open    | 打开每日任务gui  |
| /plk shop    | 打开任务币商城gui  |