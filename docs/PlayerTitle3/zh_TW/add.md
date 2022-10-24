### 新增稱號指令

> /plt title add [稱號類型] [稱號名稱] [金額] (天數) (是否隱藏) (稱號描述)

#### 稱號類型分為:
* not: 無條件
* vault: 金幣
* playerPoints: 點券
* coin: 稱號幣
* itemStack: 物品
* permission: 權限
* activity: 活動

#### 金額/數量
* 類型: 金幣,點券,稱號幣 -> 購買價格
* 類型: 物品 -> 需求數量(需主手持對應物品)
* 類型: 其他 -> 無用

#### 天數
* 稱號出售的天數,只能為正整數,0為永久

#### 是否隱藏
* false隱藏(不會顯示在plt shop中) true顯示
#### 描述
* 稱號描述可使用英文逗號 **,** 進行換行

### 額外註意事項
* [] 的為必填項  () 的為選填

### 例子

1. 新增: 白嫖者稱號 玩家點擊即可獲取永久
```
/plt title add not &e白嫖稱號 0 0 true 這是稱號描述,這是第二行
```

2. 新增: 金幣稱號  玩家需要消耗666金幣來獲取6天(需:Vault支持)
```
/plt title add vault &e金幣稱號 666 6 true 這是個金幣稱號
```

3. 新增:點券稱號 玩家需要消耗666點券來獲取6天(需:PlayerPoints支持)
```
/plt title add playerPoints &e點券稱號 666 0 false 這是個隱藏起來的點券稱號
```

4. 新增:鉆石劍稱號 玩家需要消耗鉆石劍1個來獲取永久稱號
   備註:需要手持鉆石劍來輸入該命令
```
/plt title add itemStack &e鉆石劍稱號 1 0 false 需要手持鉆石劍來輸入該命令
```

5. 新增: 稱號幣稱號: 玩家需要消耗稱號幣666來獲取6天
```
/plt title add coin &e稱號幣稱號 666 6 true 這是個稱號幣稱號
```

6. 新增: 權限稱號: 玩家有權限**test**登錄後自動獲取
```
/plt title add permission 權限稱號 test 這是個權限稱號的描述,玩家有權限**test**登錄後自動獲取
```

7. 新增: 活動稱號: 這類稱號無法購買,只能OP指令給予
```
/plt title add activity 活動稱號 0 0 true 這是個活動稱號,只能op給予
```

### 如何直接給玩家一個稱號

```
1. 新增一個稱號並給玩家30天(會增加一個隱藏稱號)
/plt player addTitle xiongliu &e新增一個給玩家的稱號 30

2. 設置一個已有的稱號ID為的1的並給玩家30天(是設置已有稱號)
/plt player setTitle xiongliu 1 30
```

### 如何在yml裏配置稱號後導入
```
1. 先配置import.yml內容

2. 執行指令/plt title import即可導入稱號
```

### 如何把現有的稱號導出成yml文件(3.1.4+)
```
1. 執行指令/plt title export

2. 現有的稱號都導出到export.yml中了

註意: 稱號的前後綴也會一起導出! 
```
