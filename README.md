# TS3AudioBot-siri
此快捷指令
基于Splamy/TS3AudioBot项目 [https://github.com/Splamy/TS3AudioBot](https://github.com/Splamy/TS3AudioBot)

网易云音乐 API[https://github.com/Binaryify/NeteaseCloudMusicApi](https://github.com/Binaryify/NeteaseCloudMusicApi)

TS3AudioBot 网易云插件[ZHANGTIANYAO1/TS3AudioBot-NetEaseCloudmusic-plugin](https://github.com/ZHANGTIANYAO1/TS3AudioBot-NetEaseCloudmusic-plugin)

以及插件 Linux 版制作[FiveHair/TS3AudioBot-NetEaseCloudmusic-plugin-UNM](https://github.com/FiveHair/TS3AudioBot-NetEaseCloudmusic-plugin-UNM)

出于打游戏时切屏切歌不方便，以及朋友不太会用命令操作。
于是想到了用 IOS 的快捷指令操作 TS3AudioBos WebAPI 

一共做了两个版本（需要修改的地方都在里面加注释了，自行修改为自己的地址）

	1、普通版，只能语音识别歌名并播放
	https://www.icloud.com/shortcuts/6894d8282a814ba485ad58f58ce1d38e
	2、接入 ChatGPT 版  可以把白话翻译为 WebAPI 可以接收的参数（推荐）
	https://www.icloud.com/shortcuts/06de61929c884fb89b5ce191650f3c2a
![image](https://github.com/jmiaob/TS3AudioBot-siri/assets/115988904/404f0f00-7989-4d03-94dc-538be538aa0e)

![image](https://github.com/jmiaob/TS3AudioBot-siri/assets/115988904/4bdf7636-748a-41cc-a28f-f35c3ff2e9dd)

![image](https://github.com/jmiaob/TS3AudioBot-siri/assets/115988904/8a5b04e5-5c91-4c03-83bd-8f53daa8b773)




本人纯业余萌新，只是自己捣鼓玩，想自己修改可以参考此 prompt，也欢迎大佬指正。
```txt
你是一个转译器,讲白话转移为标准格式，单独返回给我参数。
这是规则：
1、播放音乐和歌手:/yun/play/歌名/歌手
2、暂停:/pause
3、下一首:/yun/next
4、下一首播放歌曲:/yun/add/歌名
5、播放歌单，请返回给我:/yun/gedan/歌单名称
6、播放模式选择[0=顺序 2=随机 3=循环]:/yun/mode/播放模式
7、音量(0-100):/volume/音量
```
