### 菜单示例配置


```
# 标题
title: '&7演示菜单'
# 打开命令
openCommand: 'mc'
# 打开物品
openItem: 'clock'
# 菜单大小
size: 54
# 菜单内容 支持变量
# [message] 发送消息 [allMessage] 发送消息给全服
# [title] 发送消息 [allTitle] 发送消息给全服  格式 title:subTitle
# [actionbar] 发送消息 [allActionbar] 发送消息给全服
# [command] 执行命令 [op] op身份执行命令 [Console] 控制台执行命令
# [close] 关闭菜单
menu:
  '20':
    # 按钮坐标
    index: 20
    # 按钮名称
    name: '   &8[&c发送消息&8]'
    # 按钮材质
    material: ARROW
    lore:
      - "&f- &7点击发送消息"
    # 按钮是否附魔
    isEnchant: false
    # 按钮的自定义材质
    custom-model-data: 0
    commands:
      - '[message] 你好'
      - '[title] 大标题:小标题'
      - '[actionbar] 你好'
  '21':
    index: 21
    name: '   &8[&c执行命令&8]'
    material: ARROW
    lore:
      - "&f- &7点击回到主城"
    isEnchant: false
    custom-model-data: 0
    commands:
      - '[command] say 执行命令'
      - '[Console] say 控制台执行命令'
  '22':
    index: 22
    name: '   &8[&c点券消费&8]'
    material: ARROW
    lore:
      - "&f- &7点击点券消费"
    isEnchant: false
    custom-model-data: 0
    # 需要花费100点券才能点击
    point: 100
    commands:
      - '[command] say 你开通了vip'
      - '[allMessage] 恭喜 %player_name% 开通了点券vip'
  '23':
    index: 23
    name: '   &8[&c金币消费&8]'
    material: ARROW
    lore:
      - "&f- &7点击金币消费"
    isEnchant: false
    custom-model-data: 0
    # 需要花费100金币才能点击
    money: 100
    commands:
      - '[command] say 你开通了金币vip'
      - '[allMessage] 恭喜 %player_name% 开通了金币vip'
  '29':
    index: 29
    name: '   &8[&c只能购买3次&8]'
    material: ARROW
    lore:
      - "&f- &7点击金币购买"
      - "&f- &7限制使用三次"
    isEnchant: false
    custom-model-data: 0
    # 需要花费100金币才能点击
    money: 100
    # 限制只能使用三次本按钮
    limit: 3
    commands:
      - '[command] say 你开通了金币vip'
      - '[allMessage] 恭喜 %player_name% 开通了金币vip'
  '30':
    index: 30
    name: '   &8[&c变量条件&8]'
    material: ARROW
    lore:
      - "&f- &7变量条件支持6种符号"
      - "&f- &7 = ; !=; >; <; >=; <="
      - "&f- &7 = ; !=; 无限制"
      - "&f- &7>; <; >=; <= 必须为数字"
    isEnchant: false
    custom-model-data: 0
    # 自定义条件
    conditions:
      - '%player_name% = 米饭'
      - '%player_money% > 100'
    commands:
      - '[message] say 你点击了该按钮'
  # 分隔板 index你可以多写坐标
  pane:
    enable: true
    index: 0,1,2,3,5,6,7,8,9,17,18,26,27,35,36,44,45,46,47,48,50,51,52,53
    material: BLACK_STAINED_GLASS_PANE
    isEnchant: false
    name: "       &8[&7分割板&8]"
    lore:
      - "&7哎呀,不要随便戳人家啦"
    custom-model-data: 0

```