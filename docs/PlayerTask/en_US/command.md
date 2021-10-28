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
| playertask.delToday | Clear today's task list and all players' tasks (1.4.1+) | op |
| playertask.delShop | Delete the shop item with the corresponding id | op |
| playertask.getip | Get ip | op |
| playertask.reload | reload configuration | op |
| playertask.edit | Edit task (1.7.1+) | op |
| playertask addNpcTask | Adding npc tasks (1.6.0+) | op |
| playertask delNpcTask | DeleteNpcTask(1.6.0+) | op |
| playertask.setRarity | Edit Task Rarity (1.8.7+) | op |
| playertask.changeItem | Generate quest scrolls (1.9.0+) | op |

## Command (Admin):
| command | usage |
| ------------ | ------------ |
| /plk addDemand [target type] [number] | Add quest target (requires main hand to have item) |
| /plk addReward [reward type] [number] | Add a reward (if the reward type is an item, the master must have the corresponding item in hand)
| /plk addShop [type] [price] | Add Quest Shop item rewards (type: once: once; unlimited: infinite) | /plk addReward [type] [price] | Add Quest Shop item rewards (type: once: once; unlimited)
| /plk create [quest name] (quest type) (quest rarity) | Use gui to create tasks (recommended) |
| /plk addList [task name] [title target id] [task reward id] | Add a task using the command method |
| /plk delete [type] [corresponding id] | Use the command to delete a quest, quest target, quest reward |
| /plk view [type] | Use the gui to view and manage types, [list:task,demand:task target,reward:task reward, e.g.: /plk view list|
| /plk getToday | Execute a get today task immediately|
| /plk delToday | Clear today's task list and all players' tasks (1.4.1+)|
| /plk delShop [Corresponding ID] | Deletes the Quest Coin Shop item with the corresponding id|
| /plk getIp | Get ip|
| /plk reload | reload configuration|
| /plk edit [task id] | Use gui to edit tasks (1.7.1+) |
| /plk addNpcTask [task id] [npcId] [whether task is permanent] [number of completions possible] [cooldown] (predecessor task id) | addNpcTask(1.6.0+)|
| /plk delNpcTask [npcId] | Remove npc task (1.6.0+)|
| /plk setRarity [task id] [rarity]| Edit task rarity (1.8.7+)|
| /plk changeItem [quest id] (player name)| Generate quest scroll (1.9.0+)|

## Command (Player):
| command | use |
| ------------ | ------------ |
| /plk open | Opens the daily quest gui |
| /plk shop | open quest coin mall gui |

```
# The player executes the command, the 0 in the middle means it is executed according to the player's identity, if the player does not have permission it will fail.
/plk addReward command 0 eco#give#${player}#666
# Players execute the command, a 1 in the middle means it is executed as an op
/plk addReward command 1 eco#give#${player}#666
```

> Task types are divided into everyday (daily tasks) npc (NPC tasks) Not interchangeable
