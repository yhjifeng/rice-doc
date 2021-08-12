## Permissions
##### This plug-in default does not need to configure any permissions, the owner of the service out of the box that use
##### a lot of the following types involved do not know the low version, please use the tab reminder, 1.12 or more will automatically remind

| Permissions | Usage | Default owner |
| ------------ | ------------ | ------------ |
| playertask.addList | Add task | op |
| playertask.addDemand | Add task target | op |
| playertask.addReward | New task reward | op |
| playertask.addShop | Add a new task shop item | op |
| playertask.open | Daily quest gui | op |
| playertask.shop | Task Shop gui | op |
| playertask.create | create task | op |
| playertask.delete | delete task | op |
| playertask.view | Manage Tasks | op |
| playertask.vip | vio permissions | op |
| playertask.getToday | Get today's tasks now | op |
| playertask.delShop | Delete the task coin shop items with the corresponding id | op |
| playertask.getip | Get ip | op |
| playertask.reload | reload configuration | op |

## Command (admin):
| command | purpose |
| ------------ | ------------ |
| /plk addDemand [target type] [number] | Add quest target (requires a corresponding item in the main hand) |
| /plk addReward [reward type] [number] | Add a reward (if the reward type is an item, the master must have the corresponding item in hand)
| /plk addShop [type] [price] | Add QuestShop item rewards (type: once: once; infinite: infinite) | /plk addReward [type] [price] | Add QuestShop item rewards (type: once: once; infinite)
| /plk create [task name] | Use gui to create tasks (recommended) |
| /plk addList [task name] [title target id] [task reward id] | Add a task using the command method |
| /plk delete [type] [corresponding id] | Use the command to delete a quest,quest target,quest reward |
| /plk view [type] | Use the gui to view and manage types, [list:task,demand:task target,reward:task reward, for example: /plk view list|
| /plk getToday | Execute the get today task procedure once|
|/plk delShop [corresponding ID] | Delete the task coin shop items with the corresponding id|
|/plk getIp | Get ip|
|/plk reload | reload the configuration|

## Command (player):
| command | use |
| ------------ | ------------ |
| /plk open | Open the daily quest gui |
| /plk shop | open quest coin mall gui |