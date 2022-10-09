## Example
Description:
```
The logic of this plugin is:
1. first have a mission objective and a mission reward
2. then multiple quest objectives and quest rewards are combined to create a quest
3. the quests are now divided into two categories, one for npc and one for daily quests (1.6.0+)
4. note, in order to be compatible with rpg items, please make sure to keep the durability of the item you are holding full, otherwise you will have the problem of synthesizing the item but the quest is not +1, because the durability is not matched.
```
Suppose we want to create a quest
Mission Name: Newbie Mission

Requirement 1: Synthesize 3 diamond blocks
Requirement 2: Dig 10 diamond mines

Reward 1: 1 diamond helmet
Reward 2: 100 gold coins

Step 1. New: Mission Objectives
```
Main handheld diamond block input
/plk addDemand craftItem 3
The main hand is holding a diamond mine.
/plk addDemand blockBreak 10
```

Step 2. New: Mission Reward
```
The master holds the diamond helmet and enters
/plk addReward itemStack 1
Type directly into
/plk addReward vault 100
```

Step 3. Add a daily task
```
/plk create newbie task everyday
```

Step 3. Add new NPC quests (1.6.0+)
```
/plk create NewbieQuest npc
```

Special reminder:
```
The first time you create a quest, it won't be available in /plk open, you need /plk gettoday to get today's quests.
After that the daily quests will be refreshed at 00:00 every day (npc quests will not be refreshed)
```

This will complete a quest, and the above quest objectives and rewards can be reused indefinitely once they are created.
## Screenshot description
![4oeBcj.png](https://z3.ax1x.com/2021/09/30/4oeBcj.png)
![4oeDjs.png](https://z3.ax1x.com/2021/09/30/4oeDjs.png)
![4oe03Q.png](https://z3.ax1x.com/2021/09/30/4oe03Q.png)
![4oesun.png](https://z3.ax1x.com/2021/09/30/4oesun.png)
![4oeyBq.png](https://z3.ax1x.com/2021/09/30/4oeyBq.png)
![4oeh34.png](https://z3.ax1x.com/2021/09/30/4oeh34.png)
![4oegEV.png](https://z3.ax1x.com/2021/09/30/4oegEV.png)
![4oeR4U.png](https://z3.ax1x.com/2021/09/30/4oeR4U.png)
![4oe2NT.png](https://z3.ax1x.com/2021/09/30/4oe2NT.png)
![4oe4gJ.png](https://z3.ax1x.com/2021/09/30/4oe4gJ.png)
![4oeqUK.png](https://z3.ax1x.com/2021/09/30/4oeqUK.png)
![4oeouR.png](https://z3.ax1x.com/2021/09/30/4oeouR.png)