## 歡迎對接本插件開發更多附屬插件~
你可以基於稱號來自定義擴展,你可以初始化一個或者多個稱號,然後達到什麽條件後可以玩家獲取這個稱號
例如: 你可以設置個 等級達人稱號  然後監聽玩家等級到了多少級就給玩家這個稱號


## 使用方法

#### 初始化jar
下載代碼中的PlayerTitle-2.5.9.jar文件導入你的項目中
或者使用maven引入依賴(本地機器私庫,有時候不在線)

```
<repositories>
    <repository>
        <id>minecraft</id>
        <url>http://23.224.140.154:18208/repository/minecraft/</url>
    </repository>
</repositories>

<dependency>
  <groupId>com.handy.playertitle</groupId>
  <artifactId>PlayerTitle</artifactId>
  <version>2.7.9</version>
</dependency>
```

1. 在附屬插件初始化時候新增關聯的稱號
2. 並把稱號唯一id保存在附屬插件的yml或者數據庫中進行永久保存
3. 根據玩家名和這個稱號的唯一id將稱號給予玩家
4. 具體查詢: [開源地址](https://github.com/handy-git/PlayerTitleVersions "開源地址")  ApiTest類   或者 [javadoc](https://handy-git.github.io/PlayerTitleVersions/ "javadoc")