### Version information

### Known bugs (currently known but unresolved bugs will be displayed here)
1. plugins do not use yum such plugins for hot loading!
2. mission target, some items held in the hand and put down is a different item, so it can not be detected, it is recommended here try not to use these special items as the mission target, for example: red stone powder, railroad tracks, seeds ...
3. <=4.7 version of MythicMobs please use the compatible version of MCBBS post
#### If you encounter errors, or plug-in conflicts and other problems, please add group feedback

------------
### 1.8.5
**August 11, 2021:**
1. **Change** abandoned compatible < MythicMobs4.7 version, if you want to use, please mcbbs post download compatible version

**1.8.5 upgrade assistant**
- Configuration file compared to 1.8.4 version no change, direct replacement jar can be

### 1.8.4
**August 7, 2021:**
1. **Fix** some issues with MythicMobs

**1.8.4 upgrade small helper**
- The configuration file has no changes compared to 1.8.3, just replace the jar directly

### 1.8.3
**July 26th, 2021:**
1. **optimized** compatible with version 1.17 of the Chinese, if you are upgrading remember to delete the zhch.json in the configuration

**1.8.3 upgrade assistant**
- Configuration file compared to version 1.8.1 no change, directly replace the jar can be

### 1.8.1
**July 20, 2021:**
1. **Fix** Error on player command execution in the background
2. **Optimization** Code structure optimization
3. **Optimize** disable adding mm kill task when no mm is loaded

**1.8.1 upgrade small assistant**
- Configuration file compared to version 1.8.0 no change, direct replacement jar can be

#### 1.8.0
**July 03, 2021**
1. **New** command/plk convert mysql(convert sqlite data to mysql)
2. **New** command/plk convert sqlite(convert mysql data to sqlite)
> Please try to convert when no player is online, and restart the server after the conversion operation.
3. **Optimization** Improve custom item storage serialization (in human terms, fix the reward rpg items not stacking properly)

#### 1.8.0 update small assistant
- Configuration file compared to version 1.7.2 without any changes, directly replace the jar can be

#### 1.7.2
**26 June 2021**.
1. **Optimized** Compatible with both low and high versions of mm now

#### 1.7.2 update small helper
- Configuration file compared to version 1.7.0 without any changes, direct replacement of jar can be

#### 1.7.0
**June 13, 2021**
1. **New** Compatible with version 1.17

#### 1.7.0 update small assistant
- Configuration file compared to version 1.6.8 without any changes, direct replacement of jar can be

#### 1.6.8
**04 April 04, 2021**
1. **Optimization** Now the public version is not limited to create 10 tasks, you can create unlimited tasks
1. **Optimization** Now the public version is no longer limited to the number of rewards you can get if you have playertask.vip access

#### 1.6.8 update small assistant
Configuration file compared to version 1.6.7 without any changes, directly replace the jar can be

#### 1.6.7
**March 25, 2021**
1. **Fix** /plk view list page flip error fixed

#### 1.6.7 update small helper
The configuration file has no changes compared to version 1.6.6, just replace the jar directly

#### 1.6.6
**March 14, 2021**
1. **Optimization** Add index of player task progress table to mysql storage (performance improvement for 100 people service)

#### 1.6.6 update small assistant
Configuration file compared to version 1.6.5 without any changes, direct replacement jar can be

#### 1.6.5
**February 20, 2021**
1. **Optimization** Optimize some code

#### 1.6.5 update small assistant
Configuration file compared to version 1.6.4 without any changes, direct replacement of jar can be

#### 1.6.4
**02/18/2021**.
1. **New** monster.yml configuration file used to translate the name of the normal monster kill, how to use the comments inside
2. **New** npc quest page add reminders, and you can right click to see the details of the quest
3. **New** /plk open can be set to turn on or off the button to /plk shop
4. **New** button to go to/plk open is added to /plk shop
5. **Optimized** The monster type of killing normal monsters is now automatically alerted

#### 1.6.4 update small assistant
Re-generate or manually fill in the following content into the old config and language files
New section in config:
```
# New town button for mission coin shop
shop:
  # The location to be displayed in the mission gui
  index: 45
  # Whether to display
  enable: true
  # Button material
  material: CHEST
```
Language file has a new change section:
Added under taskNpc node
```
taskNpc:
  help:
    name: "&eNpc task system"
    lore:
      - ''
      - '&c&l>> Mouse&a left click&c&l to complete the task!'
      - '&c&l>> Mouse&a middle button&c&l click to submit quest item!'
      - '&c&l>> Mouse&a right click&c&l to view quest requirements and rewards!'
```

#### 1.6.3
**February 17, 2021**
1. **New** Task refresh button now supports point coupons
2. **New** Task refresh times support custom permissions corresponding to the number of times now
3. **Fix** Cat terminal 1.12 /plk view npc open blank problem

#### 1.6.3 update small assistant
Regenerate or manually fill in the following contents to the old config and language files
If your server only uses vouchers or gold, you can remove the extra lore and set the price to 0.
The config change section:
```
# Refresh button
refresh:
  # Position in the task gui
  index: 49
  # Whether to display
  enable: true
  # How many coins to spend, 0 is not consumed, Vault is required
  cost: 666
  # How many points to spend, 0 is not consumed, PlayerPoints are required
  points: 666
  # The number of times you can refresh per person per day, restart the server or refresh at 0:00 the next day
  # Default is default:3 which means 3 times, if you have playertask.vip permission, you can get extra times.
  # You can add your own, the same as the ess home extension permission e.g. vip1: 10 vip2: 10
  times:
    default: 3
    vip: 5
  # Button material
  material: MAP
```
Language file change section:

```
# Refresh button log
refresh:
  name: "&a refresh task"
  lore:
    - ''
    - '&f[ &c refresh description &f]'
    - ''
    - '&c&l>> Click the button to refresh today's task!'
    - '&c&l>> If the task has already been claimed and completed!'
    - '&c&l>> Cannot proceed to refresh!'
    - ''
    - '&c&l>> Refreshable times: &a${times}'
    - ''
    - '&f[ &c refresh price &f]'
    - ''
    - '&c&l>> Gold: &a${cost}'
    - '&c&l>> Points: &a${points}'
    - ''
    - '&6>>&4>>&5>> &b${button} &6<<&4<<&5<<'
```

#### 1.6.2
**08 February 2021**
1. **FIX** Some items with nbt are not able to submit quests when re-entering the game

#### 1.6.1 update small assistant
Configuration file compared to version 1.6.1 without any changes, direct replacement jar can be

#### 1.6.1
**February 07, 2021**
1. **Fix** the problem that servers below 1.13 can't open/plk view npc page

#### 1.6.1 update small assistant
Configuration file compared to version 1.6.0 without any changes, direct replacement of jar can be

#### 1.6.0(mega update)
**February 06, 2021**
1. **New** NPC type tasks, please see the documentation for details
2. **Optimized** Plugin renamed: Daily Random Quest Adjusted to Player Quest Plugin

#### 1.6.0 update small assistant
- There are new contents in config,
- The language file in languages has also been added.
- It is recommended to delete the old one, then it will automatically regenerate the new one
- (If you don't regenerate, there will be a lot of missing language files!!!)

#### 1.5.0
**February 05, 2021**
1. **New** submission type task
2. **Optimized** New quest help display
3. **Fix** bug that invalidates killing normal monsters

#### 1.5.0 update small assistant
config has new content, language file also has new content, suggest to regenerate

#### 1.4.7
**February 05, 2021**
1. **Fix an abnormal error caused by ** mm monster without a name

#### 1.4.7 update small assistant
Configuration file compared to version 1.4.6 no change, directly replace the jar can be

#### 1.4.6
**January 14, 2021**
1. **Optimization** Optimization of some vulnerabilities caused by low versions, highly recommended upgrade

#### 1.4.6 update small assistant
Configuration file compared to version 1.4.5 without any changes, direct replacement of jar can be

### 1.4.5
**December 15, 2020:**
1. **New** New configuration to consume gold to refresh daily tasks

New in config.yml
```
# Refresh button
refresh:
  # The position to be displayed in the task gui
  index: 49
  # Whether to display
  enable: true
  # How many coins to spend, 0 is not consumed, Vault is required
  cost: 666
  # The number of refresh times per person per day, restart the server or refresh at 0:00 the next day
  times: 3
  # Button material
  material: MAP
```
New in language file:
```
# Refresh button log
refresh:
  name: "Refresh task"
  lore:
    - ''
    - '&f[ &c refresh description &f]'
    - ''
    - '&c&l>> Click the button to refresh today's task!'
    - '&c&l>> If the task has already been claimed and completed!'
    - '&c&l>> Cannot proceed to refresh!'
    - ''
    - '&c&l>> Refreshable times: &a${times}'
    - '&c&l>> Refresh price: &a${cost}'
    - ''
    - '&6>>&4>>&5>> &b${button} &6<<&4<<&5<<'
  refreshButton: "&6>>&4>>&5>> &bClick to refresh &6<&4<&5<<"
  noButton: "&6>>&4>>&5>> &c unable to refresh &6<&4<&5<<"
  # Command execution success alert
  successMsg: "&a task refresh successful"
  # Command execution failure alert
  failureMsg: "&a task refresh failed"
  notSufficientFunds: "$a balance is insufficient"
```

**1.4.5 Upgrade Assistant**
- Compared to 1.4.4 configuration file and language file have changed, suggest to regenerate

### 1.4.4
**November 27th, 2020:**
1. **New** New command /plk getip to get server ip
2. **New** New command/plk reload reload server configuration

**1.4.4 upgrade small assistant**
- Compared to 1.4.2, there is no change in the configuration file, just replace the jar directly

### 1.4.2
**November 17, 2020:**
1. **New** New command /plk delShop [ID] to delete items from mission coin store
2. **Optimized** More comprehensive display of Quest Coin Shop items

**1.4.2 upgrade small assistant**
- Suggest to regenerate the language file

### 1.4.1
**October 10, 2020:**
1. **New** New command /plk delToday Remove today's tasks and player tasks
2. **Optimized** now get daily tasks, is fixed at 00:00 pm to get

**1.4.1 Upgrade Assistant**
- Suggest to regenerate the language file

### 1.4.0
**October 8, 2020:**
1. **New** Now you can add quest type,kill normal monsters
2. **Optimization** I forgot what to optimize, but I submitted a bunch of stuff anyway

**1.4.0 upgrade assistant**
- Suggest to regenerate the language file

### 1.3.3
**August 26th, 2020:**
1. **Optimization** Now you can create kill missions directly by command
   Suppose we still want to create a mission objective - kill 5 zombie kings
   Step 1. Add a kill mission with a kill count of 5
````
/plk addDemand kill 5 SkeletalKnight
```
Finish

**1.3.3 Upgrade Assistant**
- Compared to 1.3.2, there is no change in the configuration file, just replace the jar directly

### 1.3.2
**August 21, 2020:**
1. **Fix the bug that /* /plk view list can't be opened with a kill type task error

**1.3.2 upgrade small assistant**
- Compared to 1.3.1 configuration file no change, directly replace the jar can be

### 1.3.1
**August 19, 2020:**
1. **Fix** vip permission display problem in open

**1.3.1 upgrade small assistant**
- Compared to 1.3.0 configuration file no change, directly replace the jar can be

### 1.3.0
**August 17, 2020:**
1. **New** task coin mall function, task coins are useful now
2. **New** vip privileges, players with corresponding privileges can get a custom multiplier of rewards
3. **Optimize** permission refinement

**1.3.0 upgrade assistant**
- The language file has changed, it is recommended to backup and regenerate it.
- config.yml has changed, suggest backup and regenerate

### 1.2.0
**August 7, 2020:**
1. **New** support for killing MythicMobs monster types
2. **New** /plk will appear help
3. **Optimized** Right click in /plk open will show more comprehensive quest objectives and quest rewards
4. **Optimized** More language type support [Optional Chinese Simplified:zh_CN;Chinese Traditional:zh_TW;English:en_US]

**1.2.0 Upgrade Assistant**
- The language file has changed, it is recommended to regenerate

### 1.1.5
**July 31, 2020:**
1. **Optimization** Optimization of version 1.7-1.12 Cloud Chinese and custom Chinese can be compatible to use together

**1.1.5 upgrade assistant**
- No change in other functions, just replace the jar directly

### 1.1.4
**July 29th, 2020:**
1. **Fixed** Giving item rewards can be non-normal stacking
2. **New** Quest rewards can now be customized with commands,
   Use # instead of spaces in the middle of the command, and use ${player} instead of spaces in the player variable
   For example:
```
# The player executes the command, the 0 in the middle means it is executed according to the player's identity, if the player doesn't have permission, the execution will fail
/plk addReward command 0 eco#give#${player}#666
# Players execute the command, the middle 1 means execute as op
/plk addReward command 1 eco#give#${player}#666
````

**1.1.4 Upgrade Assistant**
- Language file in languages Add command: "&f command" at line 50
- You can add it manually, or delete the language file and regenerate it

### 1.1.3
**July 28th, 2020:**
1. **Optimization** Improve compatibility with 1.7, no change in functionality, just replace the jar directly

### 1.1.2
**July 27, 2020:**
1. **optimize** the bug of duplicate registration commands, no change in functionality, just replace the jar directly

### 1.1.1
**July 26th, 2020:**
1. **optimize** jar package size, no change in functionality, just replace the jar directly

### 1.1.0
**July 26, 2020:** 1.
1. **Fix** The digging task is now invalid for precise collection
2. **Optimized** The item in the hand of the creation task reward and task target will only default to 1 now
3. **New** Send actionbar alerts when a mission is in progress (1.8+)
4. **New** Send title reminder when the task is completed (1.9+)
5. **New** task reward and task target and task list delete command
6. **New** You can view all current task list, all task reward list, all task target list in gui, and click to delete
7. **New** Now in the daily task list, you can preview the task target items, and task reward items if you right click
8. **New** search criteria in the quest target and quest reward gui
9. **New** mission objective type added **Consume** **Kill (not enabled)**
10. **Added** You can get today's task immediately by command

**1.1.0 Upgrade Assistant**
- Please make sure to delete the language file in languages and let it be generated automatically again

### 1.0.0
**July 22nd, 2020:**
1. This plugin is released