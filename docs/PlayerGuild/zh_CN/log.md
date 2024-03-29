## 版本信息


### 已知bug(目前知道但是未解决的bug会统一显示在这里)
- 无

#### 如果碰到报错,或者插件冲突等问题有请加群反馈

------------
#### 1.6.5
**2023年01月06日**
1. **新增** 公会主城现在可以配置禁止设置的黑名单世界了(例如副本世界禁止设置)

#### 1.6.5更新小助手
对比1.6.4 版本 直接替换jar即可

#### 1.6.4
**2022年12月18日**
1. **修复** 更改了显示gui的数量没有正确分页查询的问题

#### 1.6.4更新小助手
对比1.6.3 版本 直接替换jar即可

#### 1.6.3
**2022年12月13日**
1. **优化** 现在成员退出公会需要二次确定了

#### 1.6.3更新小助手
对比1.6.2 版本 直接替换jar即可

#### 1.6.2
**2022年12月10日**
1. **新增** config.yml新增显示gui的默认位置设置
2. **新增** shop.yml新增会长上架物品的lore黑名单
3. **新增** 新增API用于附属插件,具体看API javadoc
4. **优化** 没参加赛季公会战的现在登录后点击前往报名会直接打开公会活动
5. **优化** 匹配和赛季在人多的情况下优化
6. **修复** 关闭公会创建按钮还能创建的问题
7. **修复** 公会名描述等的颜色代码不在计算长度

#### 1.6.2更新小助手
对比1.6.1 版本 直接替换jar即可

#### 1.6.1
**2022年11月08日**
1. **优化** 批量插入性能处理
2. **新增** 公会公告功能
3. **优化** gui中点击增加200毫秒延迟

#### 1.6.1更新小助手
对比1.6.0 版本 直接替换jar即可

#### 1.6.0
**2022年10月30日**
1. **优化** sqlite存储优化(修复部分低版本核心报错)

#### 1.6.0更新小助手
对比1.5.9 版本 直接替换jar即可

#### 1.5.9
**2022年10月24日**
1. **新增** 可控制公会pvp的API
2. **优化** 对sqlite存储方式的优化(如有报错及时反馈我)

#### 1.5.9更新小助手
对比1.5.8 版本 直接替换jar即可

#### 1.5.8
**2022年10月14日**
1. **新增** kit.pvp可以配置公会战指令白名单

#### 1.5.8更新小助手
对比1.5.7 版本 直接替换jar即可

#### 1.5.7
**2022年09月25日**
1. **新增** signin.yml中添加签到权限配置,可根据权限获取更多奖励
2. **新增** 公会介绍,现在会长可以设置公会介绍了 内部变量 ${description}
3. **优化** 公会成员列表现在支持显示成员贡献给工会多少资金了 内部变量 ${player_guild_money}
4. **优化** 现在开始赛季公会战后,后台日志里会打印本次参赛公会名称了

#### 1.5.7更新小助手
对比1.5.6 版本   
signin.yml,open.yml,member.yml,setting.yml,语言文件有新增  
建议备份之前的重新生成

#### 1.5.6
**2022年09月18日**
1. **新增** 世界边境可以在world.yml 配置是否选用原版边境了

#### 1.5.6更新小助手
对比1.5.5 版本 直接替换jar即可

#### 1.5.5
**2022年09月11日**
1. **新增** 公会世界支持WorldEdit插件了,你可以自定义对应的模板了
2. **新增** 创建公会后可执行自定义指令了
3. **修复** 解散公会带颜色代码的现在会正确识别了
4. **优化** tab自动补全会提醒/plg me (类型)了
5. **优化** /plg me (类型) 可以直接打开对应类型的gui了,例如直接打开签到
6. **新增** 公会主城传送支持BC跨服了,注意需要在config中新增下面的配置(配置后会长需重设主城坐标)

#### 1.5.5更新小助手
对比1.5.4 版本 config.yml必须手动添加!!!(不添加或者留空默认不启用)

```
# 跨服传送标识-每个服必须跟bc里配置的一样(BC服必须先配置完这个,才能跨服)
serverName: "server"
```

#### 1.5.4
**2022年08月26日**
1. **新增** 添加是否正在公会战的API

#### 1.5.4更新小助手
对比1.5.3 版本 直接替换jar即可

#### 1.5.3
**2022年08月20日**
1. **修复** kitPvp.yml的血量设置不还原问题

#### 1.5.3更新小助手
对比1.5.2 版本 直接替换jar即可

#### 1.5.2
**2022年08月15日**
1. **修复** 1.5.1无法创建公会世界的问题

#### 1.5.2更新小助手
对比1.5.1 版本 直接替换jar即可

#### 1.5.1
**2022年08月14日**
1. **优化** 现在公平pvp的默认装备物品可以在配置里关闭掉了
2. **优化** 现在公会战会过滤掉死亡的玩家了
3. **修复** 给公会活跃资金的指令现在会不会错误解析颜色代码了

#### 1.5.1更新小助手
对比1.5.0 版本 直接替换jar即可

#### 1.5.0
**2022年07月30日**
1. **新增** /plg open列表现在新增俩按钮, 根据不同类型排序搜索和返回按钮(需重新生成/gui/open.yml文件)
2. **优化** logo商城已经上架的logo支持编辑了(需重新生成/gui/logoShop.yml)
3. **优化** 指令/plg addLogo [资金] [等级] (ID)  如果传了最后一个参数,效果为编辑对应ID的logo
4. **新增** 添加指令/plg setDefaultLogo [等级] 设置公会到了某级别后默认显示的logo
5. **优化** 现在logo支持nbt属性了哦,也就是可以用对应材质和头颅这种作为logo了
6. **新增** 添加指令/giveLogo [公会名] 手持物品设置为对应公会logo
7. **新增** 公会月度活跃上线,可以更好的体现出每月公会活跃度
8. **优化** /plg open (类型) 可以通过不同类型直接打开对应排序的公会列表
9. **修复** 兼容1.18.0版本的服务器
10. **修复** 一些特殊情况下,使用sqlite存储导致的数据库报错问题

#### 1.5.0更新小助手
对比1.4.9 版本 需重新生成 open.yml和logoShop.yml和语言文件

#### 1.4.9
**2022年07月16日**
1. **优化** 公会名称长度不在判断颜色代码
2. **优化** 支持最新的变量颜色解析
3. **修复** 偶现的赛季公会站无法开启,匹配公会战卡住等

#### 1.4.9更新小助手
对比1.4.8 版本 直接替换jar即可

#### 1.4.8
**2022年06月24日**
1. **优化** 公会任务现在一页支持10个了
2. **修复** 公会任务翻页修复正常
3. **优化** task.yml里的index节点无需配置，内置了

#### 1.4.8更新小助手
对比1.4.7 版本 直接替换jar即可

#### 1.4.7
**2022年06月19日**
1. **新增** 维护活跃度(需在config配置)
2. **新增** 指令/plg me
3. **优化** 没创建公会权限的无法看到创建公会按钮

#### 1.4.7更新小助手
对比1.4.6 版本 需要重新生成config.yml和setting.yml来加载维护活跃度系统

#### 1.4.6
**2022年06月15日**
1. **新增** 获取玩家公会战kd的api接口

#### 1.4.6更新小助手
对比1.4.5 版本 直接替换jar即可

#### 1.4.5
**2022年06月13日**
1. **优化** 更好兼容1.19

#### 1.4.5更新小助手
对比1.4.4 版本 直接替换jar即可

#### 1.4.4
**2022年05月20日**
1. **新增** 升级公会现在可添加最小公会成员数量限制
2. **新增** 公会添加每日维护资金系统
3. **优化** 公会战结束后传送方式可以选择

#### 1.4.4更新小助手
config.yml 新增(会自动生成)
```
# 公会战结束模式 default:回到玩家比赛开始前位置 lookLocation:回到观站点 spawn:回到主城
pvpEndModel: "default"
```
config.yml 每个公会升级新增 upMember和maintenanceMoney选项(不会自动生成)
```
# 公会设置 1:为等级，可以按照顺序无限扩展
guildSetting:
  # 1级
  1:
    # 公会人数上限
    totalNumber: 5
    # 公会升级需求公会资金-升级后会扣除处理
    upMoney: 1000
    # 公会升级需求公会活跃-达标才能进行升级
    upProsperityDegree: 1000
    # 公会升级需求成员数量-达标才能进行升级(设置为0为不限制)
    upMember: 2
    # 公会每日维护资金(每日00:00 按照(公会人数 * 维护资金)从公会资金里扣除,资金不足的公会掉级)
    maintenanceMoney: 0
```
setting.yml up节点的内部变量如下(不会自动生成)
```
lore:
- ''
- "&f- &7点击进行公会升级"
- ''
- '&8▪ &7公会当前等级 &a#${level} &7级'
- '&8▪ &7当前每日维护 &a#${maintenanceMoney} * 人数 &7资金'
- '&8▪ &7升级每日维护 &a${upMaintenanceMoney} * 人数 &7资金'
- '&8▪ &7升级需要 &a${upMoney} &7资金'
- '&8▪ &7当前拥有 &a${guildMoney} &7资金'
- '&8▪ &7升级需要 &a${upProsperityDegree} &7活跃'
- '&8▪ &7当前拥有 &a${guildProsperityDegree} &7活跃'
- '&8▪ &7升级需要 &a${upMember} &7玩家'
- '&8▪ &7当前拥有 &a${guildMember} &7玩家'
```

#### 1.4.3
**2022年05月14日**
1. **优化** 公会站结束不传送死亡状态的玩家

#### 1.4.3更新小助手
对比1.4.2 版本 直接替换jar即可

#### 1.4.2
**2022年05月08日**
1. **新增** 公会pvp管理可在setting.yml文件配置不生效世界

#### 1.4.2更新小助手
对比1.4.1 版本 直接替换jar即可

#### 1.4.1
**2022年04月29日**
1. **新增** 三个papi变量 具体见 [变量](PlayerGuild/zh_CN/papi)
2. **优化** 没有参加赛季公会战的登录会对会长进行提醒
3. **优化** open页面新增内部变量 赛季排名:${guild_season_rank}

#### 1.4.1更新小助手
对比1.4.0 版本 直接替换jar即可

#### 1.4.0
**2022年04月26日**
1. **修复** 公会商城的一些严重bug

#### 1.4.0更新小助手
对比1.3.9 版本 直接替换jar即可

#### 1.3.9
**2022年04月23日**
1. **优化** 一些性能优化

#### 1.3.9更新小助手
对比1.3.8 版本 直接替换jar即可

#### 1.3.8
**2022年04月19日**
1. **修复** 1.3.6导致的pvp限制无效bug

#### 1.3.8更新小助手
对比1.3.7 版本 直接替换jar即可

#### 1.3.7
**2022年04月16日**
1. **优化** config中新增配置可以控制成员的头颅皮肤加载
2. **修复** 公会升级世界规则导致的报错

#### 1.3.7更新小助手
对比1.3.6 版本 直接替换jar即可

#### 1.3.6
**2022年04月15日**
1. **优化** refresh 指令可以根据当前配置重置公会最大人数
2. **优化** 公会世界传送事件优先级提升
3. **优化** 在配置中关闭pvp管理的功能展示后该功能也关闭

#### 1.3.6更新小助手
对比1.3.5 版本 直接替换jar即可

#### 1.3.5
**2022年04月04日**
1. **修复** 公会商城logo无法下一页的问题

#### 1.3.5更新小助手
对比1.3.4 版本 直接替换jar即可

#### 1.3.4
**2022年03月31日**
1. **修复** 公会银行自定义捐赠可以捐负数..

#### 1.3.4更新小助手
对比1.3.3 版本 直接替换jar即可

#### 1.3.3
**2022年03月23日**
1. **优化** 更好的兼容1.13以下的版本
2. **新增** /plg convert [MySQL|SQLite]  转换数据源

#### 1.3.3更新小助手
对比1.3.2 版本 直接替换jar即可

#### 1.3.2
**2022年03月19日**
1. **新增** 新增指令/plg start 可以立即开启赛季公会战
2. **优化** 变量现在支持显示离线玩家的了

#### 1.3.2更新小助手
对比1.3.1 版本 直接替换jar即可

#### 1.3.1
**2022年03月19日**
1. **修复** 公会商店会长和副会长上架的物品 其他公会也看见的问题
2. **优化** 公会商店会长和副会长上架的物品 显示上架人
3. **优化** 公会商店会长和副会长上架的物品 自己点击效果为下架

#### 1.3.1更新小助手
对比1.3.0 版本 直接替换jar即可

#### 1.3.0
**2022年03月17日**
1. **新增** 公会商店会长和副会长也可以上架了
2. **新增** 公会匹配消息提醒
3. **修复** 世界规则使用指令刷新异常

#### 1.3.0更新小助手
对比1.2.9 版本 直接替换jar即可

#### 1.2.9
**2022年03月10日**
1. **优化** 现在兼容mysql低版本了
2. **优化** 现在activity.yml中的matePvpTime设置为0表示关闭公会战超时自动扣血功能

#### 1.2.9更新小助手
对比1.2.8 版本 直接替换jar即可

#### 1.2.8
**2022年03月02日**
1. **优化** 各种gui的title可以重载加载
2. **修复** 公会世界边境升级处理
3. **新增** 现在可以设置公会世界规则了(例如死亡不掉落)
4. **优化** 现在会自动补全新增配置了,1.18会保留注释,其他版本应该不会

#### 1.2.8更新小助手
对比1.2.7 版本配置文件变化如下:
注意: 1.18+的服务器会自动补全带注释,其他版本也会补全,但是注释没了
world.yml新增(可手动改或者备份后重新生成)
```
# 世界规则 可查阅 https://minecraft.fandom.com/zh/wiki/%E5%91%BD%E4%BB%A4/gamerule
gameRule:
  # 要设置为true的规则
  trueFlag:
    - 'keepInventory'
  # 要设置为false的规则
  falseFlag:
    - ''
```

#### 1.2.7
**2022年02月22日**
1. **优化** 热加载关闭的时候检查gui类型
2. **优化** 公会管理踢出成员返回公会列表
3. **新增** kitPvp.yml新增最大血量设置
4. **修复** 同一个人被邀请和主动申请导致重复加入公会
5. **修复** task.yml配置了任务后gui可显示多个
6. **优化** 没参加公会战的无法伤害参加玩家
7. **新增** 指令/plg signin [vault | point] [玩家名] 可后台签到
8. **新增** 指令/plg look可查看当前是否有开启的公会战
9. **新增** 一堆玩家公会相关变量

#### 1.2.7更新小助手
对比1.2.7 版本 kitpvp.yml新增(该功能请谨慎测试后在开启)
```
# 公会战开战后默认最大血量
maxHealth:
  # 是否开启 true开启
  enable: false
  health: 20
```

#### 1.2.6
**2022年02月21日**
1. **优化** 匹配公会战添加超时中毒惩罚-默认300秒可自定义
2. **优化** 默认装备还原皮革套
3. **修复** 公会满级后禁止升级

#### 1.2.6更新小助手
对比1.2.5 版本 activity.yml新增
```
# 匹配公会战时间-超时会自动扣血
matePvpTime: 300
matePvpTimeMsg: "&8[&c!&8] &a你中毒了，原因:你战斗太久了！"
```

#### 1.2.5
**2022年02月18日**
1. **修复** 玩家公会职位缓存处理
2. **修复** 兼容1.7

#### 1.2.5更新小助手
对比1.2.4 版本 直接替换jar即可

#### 1.2.4
**2022年02月15日**
1. **修复** 公会世界创建只有会长才可以操作
2. **修复** 公会世界传送异常

#### 1.2.4更新小助手
对比1.2.3 版本 直接替换jar即可

#### 1.2.3
**2022年02月13日**
1. **优化** 大量方法修改为异步处理
2. **修复** 赛季公会战关闭后,匹配还是提醒在赛季中不能报名的问题

#### 1.2.3更新小助手
对比1.2.2 版本 直接替换jar即可

#### 1.2.2
**2022年02月12日**
1. **优化** 公会战事件优先级调整
2. **修复** 赛季报名调整
3. **优化** 公会战结束后不传送生命<=0的玩家
4. **优化** 申请加入公会更加丝滑

#### 1.2.2更新小助手
对比1.2.1 版本 直接替换jar即可

#### 1.2.1
**2022年02月09日**
1. **新增** 可查看玩家离线时间
2. **新增** 玩家公会职务变量
3. **新增** 更多api
4. **新增** 创建公会全服提醒

#### 1.2.1更新小助手
对比1.2.0 版本  zh_cn.yml重新生成  
create.yml新增
```
# 公会创建后的发送全服通知消息，留空不发
createSucceedAllMsg: "&8[&a✔&8] &7恭喜玩家&a${player}&7创建了&a${name}&7公会"
```
menber.yml新增
```
- '&8▪ &7离线时间 &f ${last_quit_time}'
```

#### 1.2.0
**2022年02月07日**
1. **修复** 修复资金创建世界的bug
2. **优化** 开始公会战提前获取区块,避免掉下去
3. **优化** 修复资金创建世界文本描述错误
4. **新增** 强制解散公会指令/plg dissolve [公会名]
5. **新增** 创建公会名称黑名单
6. **新增** 彩色名公会需要权限
7. **新增** api新增获取玩家公会成员
8. **优化** 公会战开始血量恢复满
9. **优化** 公会任务结算时间可配置，并打印提醒
10. **新增** 公平pvp装备可自定义,除了头盔(固定多色皮革头盔进行区分)

#### 1.2.0更新小助手
对比1.1.9 版本
createWorld.yml和 activity.yml和 create.yml和zh_CN.yml和task.yml和
member.yml和config.yml都有变化 具体可看[Github](https://github.com/handy-git/PlayerGuild)

#### 1.1.9
**2022年02月05日**
1. **修复** 旧版本升级上来导致赛季公会战无法正常开启的bug
2. **修复** 赛季公会战开始后队伍装备颜色不一致问题

#### 1.1.9更新小助手
对比1.1.8 版本 直接替换jar即可

#### 1.1.8
**2022年02月04日**
1. **修复** 无法正常开关称号和任务功能的问题
2. **优化** 公会战掉线后上线可以执行/login指令
3. **优化** sqlite用户体验优化,不会报错了

#### 1.1.8更新小助手
对比1.1.7 版本 直接替换jar即可

#### 1.1.8
**2022年02月01日**
1. **新增** 现在没公会的进入游戏会提醒加入公会了
2. **修复** 设置里没开启的功能更换了位置还是之前功能问题
3. **优化** 公会战事件优先级调整,反正kitpvp中的指令异常

#### 1.1.7更新小助手
对比1.1.6 版本 config.yml新增
```
# 没有公会玩家登录后进行提醒
noGuildRemind: true
```
zh_CN.yml新增
```
noGuildRemind: "&8[&a✔&8] &a你还没有公会,&8[&a点击申请加入&8]"
```

#### 1.1.6
**2022年01月31日**
1. **优化** kitpvp现在可以设置让指令后台执行了
2. **修复** 赛季公会战不会推进的问题
3. **修复** 一些rpg物品长度过长的报错
4. **修复** 基础插件是cmi的时候观战点无效的问题

#### 1.1.6更新小助手
对比1.1.5 版本 kitpvp.yml可以重新生成

#### 1.1.5
**2022年01月26日**
1. **新增** 公会银行捐赠现在可以自定义捐赠
2. **修复** 邀请成员后头颅材质异常
3. **新增** 邀请成员同意后，邀请人收到消息提醒
4. **修复** 玩家第一个加入公会pvp保护不生效问题
5. **修复** 刚新建了公会pvp保护不生效问题
6. **修复** 公会战开始后可以延迟tp的bug

#### 1.1.5更新小助手
对比1.1.4 版本 需要重新生成bank.yml invitation.yml文件

#### 1.1.4
**2022年01月20日**
1. **优化** 赛季公会战装备颜色会重复(现在最大支持16个队伍不重复了)
2. **修复** 公会pvp使用药水伤害导致报错

#### 1.1.4更新小助手
对比1.1.3 版本 直接替换jar

#### 1.1.3
**2022年01月20日**
1. **优化** 成员管理和邀请成员列表异步获取玩家头颅
2. **修复** 公会战鼠标点着的物品比赛结束可以带出场地问题
3. **优化** 新增公会商城物品可设置限购次数
4. **优化** 新增公会商城默认可以使用的权限，默认精英+可用
5. **优化** 传送回公会主城移动灵敏度调低

#### 1.1.3更新小助手
对比1.1.2 版本 zhCn.yml，shop.yml, view.yml 重新生成

#### 1.1.2
**2022年01月18日**
1. **修复** 公会邀请现在可以翻页了
2. **修复** 公会成员和邀请列表取消加载玩家头颅
3. **修复** 公会升级称号不会自动跟着升级bug

#### 1.1.2更新小助手
对比1.1.1 版本 直接替换jar

#### 1.1.1
**2022年01月18日**
1. **新增** 公会现在可以成员pvp管理
2. **修复** 公会战场地异常
3. **优化** 匹配比赛结束后活着的人先传送到观战点，然后传送到之前位置
4. **新增** 公会现在可以主动邀请玩家加入了

#### 1.1.1更新小助手
对比1.1.0 版本 setting.yml有新增内容
```
# pvp管理
pvp:
  enable: true
  index: 31
  name: "   &8[&a设置成员PVP&8]"
  material: iron_sword
  isEnchant: false
  lore:
    - ''
    - '&8▪ 当前状态 &8[${pvpStatus}&8]'
    - ''
    - '&8▪ &7需支付 &a${price} &7公会资金'
    - '&8▪ &7你拥有 &a${money} &7公会资金'
    - ''
    - ' &8[&a✔&8] &7点击切换'
  custom-model-data: 0
  price: 100
  yesPvp: "&a开启PVP"
  noPvp: "&c禁止PVP"
  
 # 邀请成员
invitation:
  enable: true
  index: 22
  name: "     &8[&a邀请成员&8]"
  material: PLAYER_HEAD
  isEnchant: false
  lore:
    - "&f- &7点击可邀请在线玩家加入"
  custom-model-data: 0
```

#### 1.1.0
**2022年01月17日**
1. **优化** 公会战场地分类型-赛季和匹配，之前的场地默认都是匹配
2. **新增** 公会战开始可以设置提醒
3. **变更** 原指令/plg setLocation [场地名] [场地出生点名] 修改为/plg setLocation [类型] [场地名] [场地出生点名]

#### 1.1.0更新小助手
对比1.0.9 版本
activity.yml有新增内容
```
# 公会战开始后的发送通知消息
notice:
  # 范围 不发 not , 只有op接收 op , 全部玩家 all
  range: "op"
  msg: "&7公会${one} VS ${two} 匹配公会战开始了！"
```
zh_CN.yml有新增内容,建议重新生成

#### 1.0.9
**2022年01月17日**
1. **修复** 任务结算bug修复
2. **新增** 任务结算添加消息提醒
3. **修复** 查看成员时候成员被离开或者其他管理踢导致bug
4. **新增** 公会战准备阶段禁止扔东西
5. **修复** 次数不会减少修复

#### 1.0.9更新小助手
对比1.0.8 task.yml有新增内容
```
# 每周日晚上23:00发奖励
rewardMsg: "&8[&a✔&8] &7公会任务${taskName}结算，奖励公会资金:${guildMoney},公会活跃:${guildProsperityDegree}"
# 每周一早上01:00刷新任务
refreshMsg: "&8[&a✔&8] &7本周公会任务刷新了，为了公会肝起来吧!"
```

#### 1.0.8
**2022年01月16日**
1. **优化** 赛季公会战重做-现在为报名公会一起参与(activity.yml需重新生成)
2. **优化** 公平pvp添加对飞行和可以执行自定义指令(kitpvp.yml需重新生成)
3. **优化** 新增工会成员上次登录时间查看(member.yml需重新生成)
4. **优化** 现在pvp开始后直接禁止执行全部指令(op不限制)
5. **修复** 比赛中如果有掉线玩家重进后会传送到观战点,未设置会传送到世界出生点

#### 1.0.8更新小助手
activity.yml和kitpvp.yml和member.yml需重新生成

#### 1.0.7
**2022年01月13日**
1. **新增** 公会战胜利后可配置全服发送战胜消息

#### 1.0.7更新小助手
对比1.0.6 activity.yml有新增内容

```
# 公会战结束全服提醒(留空代表不发消息)
matePvpFinishAllMsg: "&a${win} &7公会在公会战中战胜了 &c${fail}"
```

#### 1.0.6
**2022年01月12日**
1. **修复** 公会战一些瓜皮玩家的蜜汁操作导致的bug

#### 1.0.6更新小助手
对比1.0.5无任何变化，直接替换jar即可

#### 1.0.5
**2022年01月12日**
1. **修复** 商城lore显示异常
2. **优化** refresh会把删除的公会称号还原回来

#### 1.0.5更新小助手
对比1.0.4无任何变化，直接替换jar即可

#### 1.0.4
**2022年01月11日**
1. **新增** 商城和lore商城物品新增需求公会等级
2. **新增** 玩家离开公会后重新加入的冷却时间(被踢不算)

#### 1.0.4更新小助手
- config.yml 增加 节点
```
# 离开公会后重新加入公会的冷却时间单位 小时
joinCooling: 6
```
- logoShop.yml shop.yml zh_CN.yml 有部分语言文件新增

#### 1.0.3
**2022年01月11日**
1. **新增** 指令/plg refresh  具体看指令介绍里
2. **新增** title.yml和task.yml增加参数 enable: true来控制是否开启
3. **修改** task.yml默认不会在自动生成任务，需要自己配置
4. **修复** 匹配准备阶段有可能报错的bug

#### 1.0.3更新小助手
- zh_CN.yml 增加/plg refresh 的help提醒文本
- title.yml和task.yml 增加参数 enable: true

#### 1.0.2
**2022年01月10日**
1. **新增** 新增大量操作贡献的api
2. **新增** 指令，take，give，set，具体看指令介绍里
3. **修复** 转移会长后，在gui中会长介绍还是之前的问题

#### 1.0.2更新小助手
- 只有zh_CN.yml有变化，可删除重新生成

#### 1.0.1
**2022年01月10日**
1. **修复** 1.0.0版本大量bug处理
2. **修复** 1.0.0版本新功能大量增加
3. **修复** pvp鼠标选中的物品也清理
4. **修复** plk任务结算和重发处理修复
5. **修复** 解散公会同时清理任务记录
6. **修复** 默认配置需求金额和属性做部分调整

#### 1.0.1更新小助手
- 全部配置文件对比1.0.1版本变化巨大
- 最好备份之前的 然后重新生成
- 数据文件.db变动不大，可以保留数据

### 1.0.0
**2022年1月2号:**
1. 本插件开始预售