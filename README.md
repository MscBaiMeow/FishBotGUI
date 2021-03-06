# FishBotGUI
  
源自 https://github.com/MscBaiMeow/FishBot  
  
此为[FishBot](https://github.com/MscBaiMeow/FishBot)的GUI版本  
采用~~巨鸡儿烂的~~易语言进行编写，仅可供Windows用户使用  
Linux用户请前往[原贴](https://github.com/MscBaiMeow/FishBot/releases)下载```AutoFish```  

## 截图 (仅供参考)
![1](https://raw.githubusercontent.com/Amazefcc233/FishBotGUI/master/images/snipaste_20190813_001417.png)
![2](https://raw.githubusercontent.com/Amazefcc233/FishBotGUI/master/images/snipaste_20190813_001716.png)

## Release 注意事项

1. ~~每次的Release中，**大概**会有两个文件。  
  一个是```AutoFishGUI.exe```，另一个是```AutoFishGUI-small.exe```。  
  两者的区别就在于，前者已包含了主文件，后者仅包含GUI启动部分，您必须手动下载[FishBot](https://github.com/MscBaiMeow/FishBot/releases)中的版本，并将其和GUI启动器放置在同一目录下，才可启动钓鱼机。~~  
  在v1.3及以后版本中，reload版本已完全代替未优化版本。以往的版本将不再给予支持。
2. 本GUI的Releases版本将跟随[FishBot](https://github.com/MscBaiMeow/FishBot/)版本。

## 启动注意事项

1. 在启动后，同目录下将会生成```autofish-gui-auto.bat```文件。若您无需配置上的更改，可直接运行此文件启动钓鱼机。
2. 如想保留原有配置文件，将```autofish-gui-auto.bat```文件改名即可。
3. 服务器ip不可为srv解析。可通过nslookup查看获得a记录地址和端口并重新填入。  
例：服主给出的服务器地址为```mc.example.com```，但通过cmd执行ping命令显示```Ping 请求找不到主机```，或是看得到ping后的ip却仍然无法进入服务器，则可能是使用了srv解析。  
通过输入命令```nslookup -q=srv _minecraft._tcp.mc.example.com```发现，```port```为```10000```，```srv hostname```为```a.example.com```，则可在启动器内服务器ip栏输入```a.example.com```，端口输入```10000```。  
若输入命令后发现```srv hostname```仍然为```mc.example.com```，那么可以```ping mc.example.com```来获取服务器的ip地址，然后填入服务器地址栏并填写端口，即可进入服务器。

### 正版用户须知

1. **从v1.4起，密码将不再被保存在本地，取代而之的是astk。安全性的确有所提高，但请您注意，使用astk登入仍有可能导致您的账户被他人利用。因此在任何时候，您都不应该泄露自己的astk和密码信息。我们已对此进行过警告，因随意传播密码/astk而导致账号被盗等行为，FishBot及FishBotGUI不承担任何责任。**
2. ***这里正版指的是国际服正版。和网易国服没有任何一丁点关系。***
3. 若想加入领域服，只需选择“领域”复选框即可，无需填写ip和端口。在钓鱼机登录后，可选择一个领域服并进入。

### 外置登录用户须知

1. **从v1.4起，密码将不再被保存在本地，取代而之的是astk。安全性的确有所提高，但请您注意，使用astk登入仍有可能导致您的账户被他人利用。因此在任何时候，您都不应该泄露自己的astk和密码信息。我们已对此进行过警告，因随意传播密码/astk而导致账号被盗等行为，FishBot及FishBotGUI不承担任何责任。**
2. 请在认证服务器一栏中填写你服务器的Yggdrasil API 认证服务器地址。
3. 统一通行证用户在认证服务器一栏中填写```https://auth2.nide8.com:233/($服务器ID)/```。```($服务器ID)```可为注册URL的32位ID。
  若注册地址为```https://login2.nide8.com:233/1234567890abcdef1234567890abcdef/loginreg```，则服务器id为```1234567890abcdef1234567890abcdef```。
4. 事实上并没有打算考虑统一通行证。能用便是缘分。用不了也不打算兼容。
5. 多用户可在钓鱼机登入后选择一个用户并进入服务器。

## 鸣谢

- [go-mc](https://github.com/Tnze/go-mc)
- [FishBot](https://github.com/MscBaiMeow/FishBot)
- [Miaoscraft](https://github.com/miaoscraft/)
- [易语言 - 未闻花名UI](https://bbs.125.la/home.php?mod=space&uid=378021)
- [Tsuk1ko/CQ-picfinder-robot的模版](https://github.com/Tsuk1ko/CQ-picfinder-robot)
