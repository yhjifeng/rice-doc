## Permissions
##### This plugin does not require any permissions to be configured by default, the service owner can use it out of the box
##### Many of the following types are not known. Please use the tab to remind you of low versions, 1.12 or above will be automatically reminded.

| Permissions | Usage | Default owner |
| ------------ | ------------ | ------------ |
| playertask.addList | Add task | op |
| playertask.addDemand | Add task target | op |
| playertask.addReward | Add a new task reward | op |
| playertask.addShop | Add a new task shop item | op |
| playertask.open | Daily quest gui | op |
| playertask.shop | Task Shop gui | op |
| playertask.create | Create a task | op |
| playertask.delete | Delete a task | op |
| playertask.view | Manage Tasks | op |
| playertask.vip | vio permissions | op |
| playertask.getToday | Get today's tasks now | op |
| playertask.delShop | Delete the task coin shop item with the corresponding id | op |
| playertask.getip | Get ip | op |
| playertask.reload | reload configuration | op |
| playertask.edit | Edit task | op |
| playertask.setRarity | edit task rarity 1.8.7+) | op |

## Command (Admin):
| command | use |
| ------------ | ------------ |
| /plk addDemand [target type] [number] | Add quest target (requires main hand to have corresponding item) |
| /plk addReward [Reward Type] [Number] | Add a reward (if the reward type is an item, the master must have the corresponding item in hand)
| /plk addShop [type] [price] | Add Quest Shop item rewards (type: once: once; unlimited: infinite) | /plk addReward [type] [price] | Add Quest Shop item rewards (type: once: once; unlimited)
| /plk create [task name] | Use gui to create tasks (recommended) |
| /plk addList [task name] [title target id] [task reward id] | Add a task using the command method |
| /plk delete [type] [corresponding id] | Use the command to delete a quest, quest target, quest reward |
| /plk view [type] | Use the gui to view and manage types, [list:task,demand:task target,reward:task reward, e.g.: /plk view list|
| /plk getToday | Execute the get today task once immediately|
| /plk delShop [corresponding ID] | Delete the task coin shop item with the corresponding id|
|/plk getIp | Get ip|
|/plk reload | Reload the configuration|
|/plk edit [task id] | Use gui to edit tasks |
|/plk setRarity [quest id] [rarity]| Edit quest rarity (1.8.7+) ｜

## Command (Player):
| command | use |
| ------------ | ------------ |
| /plk open | Open daily quest gui |
| /plk shop | open quest coin mall gui |