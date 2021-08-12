## Example
Description:
```
The logic of this plugin is:
1. first have a mission goal and mission reward
2. then multiple quest objectives and quest rewards are combined to create a quest
3. the task is now divided into two categories, a npc task, a daily task (1.6.0 +)
4. note, in order to be compatible with rpg items, so please be sure to keep the durability of the handheld items for full, otherwise there will be synthesized items but the task did not +1 problem, that is because the durability did not match the
````
Suppose we want to create a task
Task name: &f[&eNewbie task&f]

Requirement 1: Synthesize 3 diamond blocks
Requirement 2: Dig 10 diamond mines

Reward 1: 1 diamond helmet
Reward 2: 100 gold coins

Step 1. New: Mission Objective
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
/plk create &f[&e newbie task&f] everyday
```

Step 3. Add new NPC quests (1.6.0+)
```
/plk create &f[&e newbie quest&f] npc
```

Special reminder:
```
The first time you create a task /plk open will not have, you need /plk gettoday into get today's task
After that, the daily tasks will be refreshed automatically at 00:00 every day (npc tasks will not be refreshed)
````


So a task is completed, the above task objectives and task rewards can be infinitely reused as long as they are created.
## Screenshot description
[![WXeGxP.png](https://z3.ax1x.com/2021/07/30/WXeGxP.png)](https://imgtu.com/i/WXeGxP)
[![WXe82t.png](https://z3.ax1x.com/2021/07/30/WXe82t.png)](https://imgtu.com/i/WXe82t)
[![WXeQ5d.png](https://z3.ax1x.com/2021/07/30/WXeQ5d.png)](https://imgtu.com/i/WXeQ5d)
[![WXe38I.png](https://z3.ax1x.com/2021/07/30/WXe38I.png)](https://imgtu.com/i/WXe38I)
[![WXe1PA.png](https://z3.ax1x.com/2021/07/30/WXe1PA.png)](https://imgtu.com/i/WXe1PA)
[![WXedaQ.png](https://z3.ax1x.com/2021/07/30/WXedaQ.png)](https://imgtu.com/i/WXedaQ)
[![WXetr8.png](https://z3.ax1x.com/2021/07/30/WXetr8.png)](https://imgtu.com/i/WXetr8)
[![WXeYKf.png](https://z3.ax1x.com/2021/07/30/WXeYKf.png)](https://imgtu.com/i/WXeYKf)
[![WXeNqS.png](https://z3.ax1x.com/2021/07/30/WXeNqS.png)](https://imgtu.com/i/WXeNqS)
[![WXeaVg.png](https://z3.ax1x.com/2021/07/30/WXeaVg.png)](https://imgtu.com/i/WXeaVg)
[![WXeDGn.png](https://z3.ax1x.com/2021/07/30/WXeDGn.png)](https://imgtu.com/i/WXeDGn)
[![WXeBPs.png](https://z3.ax1x.com/2021/07/30/WXeBPs.png)](https://imgtu.com/i/WXeBPs)