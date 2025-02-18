<p align="center">
  <a href="https://github.com/KimigaiiWuyi/GenshinUID/"><img src="https://s2.loli.net/2022/01/31/kwCIl3cF1Z2GxnR.png" width="256" height="256" alt="GenshinUID"></a>
</p>
<h1 align = "center">GenshinUID</h1>
<h4 align = "center">♾️基于<a href="https://github.com/Ice-Cirno/HoshinoBot" target="_blank">HoshinoBot</a>/<a href="https://github.com/nonebot/nonebot2" target="_blank">NoneBot2</a>/<a href="https://bot.q.qq.com/wiki/#" target="_blank">QQ官方频道Bot</a>的原神多功能插件♾️</h4>
<div align = "center">
        <a href="https://github.com/KimigaiiWuyi/GenshinUID/wiki" target="_blank">安装文档</a> &nbsp; · &nbsp;
        <a href="https://github.com/KimigaiiWuyi/GenshinUID/wiki#%E4%B8%A8%E6%9F%A5%E8%AF%A2%E6%A8%A1%E5%9D%97%E6%8C%87%E4%BB%A4%E5%88%97%E8%A1%A8" target="_blank">指令列表</a> &nbsp; · &nbsp;
        <a href="https://github.com/KimigaiiWuyi/GenshinUID/wiki#%E4%B8%A8%E5%B8%B8%E8%A7%81%E9%97%AE%E9%A2%98qa">常见问题</a>
</div>
<p align="center">
  <a><img src="https://s2.loli.net/2022/02/01/QlS4piWXw5rZO3D.png"></a>
</p>


## 丨我该如何安装该插件？

+ 如果你使用的是[Go-cqhttp](https://github.com/Mrs4s/go-cqhttp) & [HoshinoBot](https://github.com/Ice-Cirno/HoshinoBot)，**安装方法查看[此处](https://github.com/KimigaiiWuyi/GenshinUID/wiki#%E4%B8%A8%E5%AE%89%E8%A3%85hoshinobot-)**。
+ 如果你使用的是[Go-cqhttp](https://github.com/Mrs4s/go-cqhttp) & [NoneBot2](https://github.com/nonebot/nonebot2)，**安装方法查看[此处](https://github.com/KimigaiiWuyi/GenshinUID/wiki#%E4%B8%A8%E5%AE%89%E8%A3%85nonebot2)**。（**开发者正在使用**）

+ 如果你想在QQ官方的频道Bot使用此插件，你需要**做好以下准备**：
  - 拥有QQ频道机器人的开发者账号（类型：私域）
  - 拥有已经备案好的服务器地址（视情况后期官方放开本地图片发送而定）
  - **腾讯频道Bot官方的文档**，查看[此处](https://bot.q.qq.com/wiki/#)
  - 安装方法：基于官方的[PythonSDK](https://github.com/tencent-connect/botpy)，本插件的安装方法可自行摸索。

## 丨我该如何获取Cookies？[#92](https://github.com/KimigaiiWuyi/GenshinUID/issues/92)（[@RemKeeper](https://github.com/RemKeeper)）

```
var cookie=document.cookie;
var Str_Num = cookie.indexOf('_MHYUUID=');
cookie ='添加 '+cookie.substring(Str_Num);
var ask=confirm('Cookie:'+cookie+'\n\n按确认，然后粘贴发送给机器人');
if(ask==true)
    {copy(cookie);
        msg=cookie}
else
    {msg='Cancel'}
```

1. 复制上面全部代码，然后打开https://bbs.mihoyo.com/ys/
2. 在页面上右键检查或者Ctrl+Shift+i
3. 选择控制台（Console），粘贴，回车，在弹出的窗口点确认（点完自动复制）
4. 然后在和机器人的私聊窗口，粘贴发送即可

**警告：Cookies属于个人隐私，其效用相当于账号密码，请勿随意公开！**

## 丨获取米游社Stoken([AutoMihoyoBBS](https://github.com/Womsxd/AutoMihoyoBBS#%E8%8E%B7%E5%8F%96%E7%B1%B3%E6%B8%B8%E7%A4%BECookie))
**前提**：已经添加过米游社Cookies，并且已经绑定过uid(仅用于米游社币的获取)
```sh
var cookie=document.cookie;
var ask=confirm('Cookie:'+cookie+'\n\nDo you want to copy the cookie to the clipboard?');
if(ask==true){copy("添加 stoken" + cookie);msg=cookie}else{msg='Cancel'}
```

1. 复制上面全部代码，然后打开http://user.mihoyo.com/
2. 在页面上右键检查或者Ctrl+Shift+i
3. 选择控制台（Console），粘贴，回车，在弹出的窗口点确认（点完自动复制）
4. 然后在和机器人的私聊窗口，粘贴发送即可

**警告：Cookies属于个人隐私，其效用相当于账号密码，请勿随意公开！**

## 丨感谢

- [PaimonBot](https://github.com/XiaoMiku01/PaimonBot) - 插件原始代码来自于它
- [YuanShen_User_Info](https://github.com/Womsxd/YuanShen_User_Info) - 米游社API来自于它
- *[MiniGG](https://www.minigg.cn/)* - Wiki API来自于它
- [@MingxuanGame](https://github.com/MingxuanGame) - [Nonebot2-beta1](https://github.com/KimigaiiWuyi/GenshinUID/tree/nonebot2-beta1)分支新建与维护
- [@shirokurakana](https://github.com/shirokurakana) - [Nonebot2-beta1分支的修复与优化](https://github.com/KimigaiiWuyi/GenshinUID/pull/118)
- [@AMEKENN](https://github.com/AMEKENN) - 米游社签到部分的代码指导
- [@lgc233](https://github.com/lgc2333) - 众多优秀PR贡献
- [@RemKeeper](https://github.com/RemKeeper) - 简易Cookies获取文档
- [@珊瑚宫千花](https://space.bilibili.com/398528056) - 角色别名Json提供
- [@wudifeixue](https://github.com/wudifeixue) - PR贡献 & Bug报告
- [@ZhouYingSASA](https://github.com/ZhouYingSASA) - PR贡献 & Bug报告

## 丨其他

+ 如果对本插件有功能建议&Bug报告，欢迎提Issuse & Pr，每一条都会详细看过
+ 如果本插件对你有帮助，不要忘了点个Star~
+ 本项目仅供学习使用，请勿用于商业用途
+ [爱发电](https://afdian.net/@KimigaiiWuyi)
+ [GPL-3.0 License](https://github.com/KimigaiiWuyi/GenshinUID/blob/main/LICENSE) © [@KimigaiiWuyi](https://github.com/KimigaiiWuyi)
