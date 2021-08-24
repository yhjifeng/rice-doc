## Welcome to dock this plug-in to develop more subsidiary plug-ins ~
You can customize the extension based on the title, you can initialize one or more titles, and then after reaching what conditions the player can get the title
For example: you can set a level master title and then listen to the player's level to give the player this title


## How to use

#### initialize the jar
Download the PlayerTitle-2.5.9.jar file from the code and import it into your project
Or use maven to introduce dependencies (local machine private library, sometimes not online)

```
<repositories>
   <repository>
      <id>player-title</id>
      <url>https://raw.githubusercontent.com/handy-git/PlayerTitleVersions/master/repo</url>
   </repository>
</repositories>

<dependency>
  <groupId>com.handy.playertitle</groupId>
  <artifactId>PlayerTitle</artifactId>
  <version>2.8.1</version>
</dependency>
```

1. add the associated title to the dependency plugin during initialization
2. and save the unique id of the title in the yml or database of the dependency plugin for permanent storage
3. according to the player name and the unique id of the title will be given to the player
4. Specific inquiries: [Open Source Address](https://github.com/handy-git/PlayerTitleVersions "开源地址")  ApiTest class or [javadoc](https://handy-git.github.io/PlayerTitleVersions/ "javadoc")