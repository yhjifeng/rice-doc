### 新增称号指令

> /plt title add [称号类型] [称号名称] [金额] (天数) (是否隐藏) (称号描述)

#### 称号类型分为:
* not: 无条件
* vault: 金币 
* playerPoints: 点券 
* coin: 称号币
* itemStack: 物品
* permission: 权限
* activity: 活动

#### 金额/数量
* 类型: 金币,点券,称号币 -> 购买价格
* 类型: 物品 -> 需求数量(需主手持对应物品)
* 类型: 其他 -> 无用

#### 天数
* 称号出售的天数,只能为正整数,0为永久

#### 是否隐藏
* false隐藏(不会显示在plt shop中) true显示
#### 描述
* 称号描述可使用英文逗号 **,** 进行换行

### 额外注意事项
* [] 的为必填项  () 的为选填

### 例子

1. 新增: 白嫖者称号 玩家点击即可获取永久
```
/plt title add not &e白嫖称号 0 0 true 这是称号描述,这是第二行
```

2. 新增: 金币称号  玩家需要消耗666金币来获取6天(需:Vault支持)
```
/plt title add vault &e金币称号 666 6 true 这是个金币称号
```

3. 新增:点券称号 玩家需要消耗666点券来获取6天(需:PlayerPoints支持)
```
/plt title add playerPoints &e点券称号 666 0 false 这是个隐藏起来的点券称号
```

4. 新增:钻石剑称号 玩家需要消耗钻石剑1个来获取永久称号
   备注:需要手持钻石剑来输入该命令
```
/plt title add itemStack &e钻石剑称号 1 0 false 需要手持钻石剑来输入该命令
```

5. 新增: 称号币称号: 玩家需要消耗称号币666来获取6天
```
/plt title add coin &e称号币称号 666 6 true 这是个称号币称号
```

6. 新增: 权限称号: 玩家有权限**test**登录后自动获取
```
/plt title add permission 权限称号 test 这是个权限称号的描述,玩家有权限**test**登录后自动获取
```

7. 新增: 活动称号: 这类称号无法购买,只能OP指令给予
```
/plt title add activity 活动称号 0 0 true 这是个活动称号,只能op给予
```

### 如何直接给玩家一个称号

```
1. 新增一个称号并给玩家30天(会增加一个隐藏称号)
/plt player addTitle xiongliu &e新增一个给玩家的称号 30

2. 设置一个已有的称号ID为的1的并给玩家30天(是设置已有称号)
/plt player setTitle xiongliu 1 30
```

### 如何在yml里配置称号后导入
```
1. 先配置import.yml内容

2. 执行指令/plt title import即可导入称号
```

### 如何把现有的称号导出成yml文件(3.1.4+)
```
1. 执行指令/plt title export

2. 现有的称号都导出到export.yml中了

注意: 称号的前后缀也会一起导出! 
```
