## 例子
說明:
```
本插件的邏輯是:
1. 首先有了任務目標和任務獎勵
2. 然後將多個任務目標和任務獎勵組合起來創建出一個任務
3. 任務現在分為倆類,一種npc任務,一種每日任務(1.6.0+)
4. 註意,為了兼容rpg物品,所以請一定要保持手持物品的耐久為滿,不然會出現合成了物品但是卻任務沒+1的問題,那是因為耐久沒匹配到
```
假設我們要創建一個任務
任務名稱: &f[&e新手任務&f]

要求1: 合成 3個鉆石塊
要求2: 挖掘10個鉆石礦

獎勵1: 1個鉆石頭盔
獎勵2: 100金幣

步驟一. 新增: 任務目標
```
主手持鉆石塊輸入
/plk addDemand craftItem 3
主手持鉆石礦輸入
/plk addDemand blockBreak 10
```
步驟二. 新增: 任務獎勵
```
主手持鉆石頭盔輸入
/plk addReward itemStack 1
直接輸入
/plk addReward vault 100
```

步驟三. 新增每日任務
```
/plk create &f[&e新手任務&f] everyday
```

步驟三. 新增NPC任務(1.6.0+)
```
/plk create &f[&e新手任務&f] npc
```

特別提醒:
```
第一次創建好任務後/plk open中不會有,需要/plk gettoday進獲取今日任務
之後每天00:00會自動刷新每日任務(npc任務不會刷新)
```


這樣一個任務就完成了,上面的任務目標和任務獎勵只要創建了就可以無限的復用.
## 截圖說明
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