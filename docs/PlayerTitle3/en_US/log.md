## Version information

### Known bugs (currently known but unresolved bugs will be shown here in one place)
> 1. /plt view shop command conflicts with [crazycrate](https://www.mcbbs.net/thread-688445-1-1.html) version 1.7.4

#### If you encounter errors, or plug-in conflicts and other problems, please add the group feedback

------------
#### 3.1.4
**October 24, 2022**
1. **New** New command to export title to yml /plt title export
2. **Optimization** sqlite storage optimization (if low version encounter error please even feedback)

#### 3.1.4 update small assistant
Compared to 3.1.3 version directly replace the jar can be

#### 3.1.3
**October 14, 2022**
1. **New** title support for papi variable parsing
2. **Optimized** mysql8+ for better support

#### 3.1.3 update for small helpers
Compare to 3.1.2 version Just replace the jar directly

#### 3.1.2
**24 September 2022**
1. **New** title description support for papi variable parsing

#### 3.1.2 update of the little helper
Compared to 3.1.1 version just replace the jar directly

#### 3.1.1
**20 August 2022**
1. **New** Add keyword blacklist to custom title
2. **FIXED** Changed plt view open [player] page number exception
3. **New** api to determine if a player has a corresponding title

#### 3.1.1 update of the small helper
Compare to version 3.1.0. Just replace the jar directly.

#### 3.1.0
**16 August 2022**
1. **New** title buff is now compatible with AttributeSystem

#### 3.1.0 update small assistant
Compared to version 3.0.9 just replace the jar directly

#### 3.0.9
**08/14/2022** 1.
1. **New** Name compatible variables

#### 3.0.9 update small assistant
Compared to 3.0.8 version directly replace the jar can be

#### 3.0.8
**August 03, 2022**
1. **optimized** reload command alert

#### 3.0.8 update small assistant
Compare to version 3.0.7 Direct jar replacement

#### 3.0.7
**July 28, 2022**
1. **Fix** 1.18.0 server with possible error reporting
2. **Optimize** occasional table locking bug in sqlite

#### 3.0.7 update small assistant
Compare to 3.0.6 version Directly replace the jar can be

#### 3.0.6
**July 17, 2022**
1. **Added** /plt shop custom to open custom title page directly
2. **New** isChat chat format can be configured (that space can be matched)
3. **New** New clear command to clean up the corresponding player title data and corresponding type of data
4. **FIX** Fix the problem that the permission title description cannot be added directly

#### 3.0.6 update small assistant
Compared to version 3.0.5 config can add the following configuration

```
# Chat display title format
isChatFormat: " "
```

#### 3.0.5
**06 July 2022**
1. **Fix** custom configuration in shop.yml uses parameters from open.yml
2. **Optimization** tab patching optimization

#### 3.0.5 update small assistant
Compare to 3.0.4 version, just replace the jar directly.

#### 3.0.4
**July 02, 2022**
1. **Fix** Fix the problem of invalid custom title length limit

#### 3.0.4 update small assistant
Compare to version 3.0.3 Directly replace the jar

#### 3.0.3
**June 24, 2022**
1. **Fix** Fix change title name exception

#### 3.0.3 update small assistant
Compare to version 3.0.2 Directly replace the jar

#### 3.0.2
**June 14, 2022**
1. **Optimization** Fix some special cases where the buff information of 2.x cannot be synchronized to 3.x

#### 3.0.2 update small assistant
Compare with 3.0.1 version, just replace the jar directly

#### 3.0.1
**June 13, 2022**
1. **Optimization** Better compatibility with 1.19

#### 3.0.1 update small assistant
Compare to 3.0.0 version Just replace the jar directly

#### 3.0.0
**May 22, 2022**
1. **Optimization** Command system change [**Commands and permissions**](PlayerTitle3/zh_CN/command)
2. **Optimization** Now fully customizable gui 100% of the time
3. **Optimization** Now you can use the command to quickly configure the title in yml and then import it
4. **Optimized** Removed some of the very low usage features
5. **Optimization** The gui style now looks better
6. **Optimization** The player customization function is integrated into the title mall

#### 3.0.0 update small assistant
- Configuration file compared to 2.x has a huge change, except for the database file, all other deleted to let regenerate (first backup)
- Upgrade 3.0.0 is indifferent to players, data will not be lost, perfectly compatible