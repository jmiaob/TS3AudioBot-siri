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
	https://www.icloud.com/shortcuts/a8a531e2909e4f7c90bf4e31a0a598ac
![image](https://github.com/jmiaob/TS3AudioBot-siri/assets/115988904/404f0f00-7989-4d03-94dc-538be538aa0e)

![image](https://github.com/jmiaob/TS3AudioBot-siri/assets/115988904/4bdf7636-748a-41cc-a28f-f35c3ff2e9dd)

![image](https://github.com/jmiaob/TS3AudioBot-siri/assets/115988904/8a5b04e5-5c91-4c03-83bd-8f53daa8b773)




本人纯业余萌新，只是自己捣鼓玩，想自己修改可以参考此 prompt，也欢迎大佬指正。
```txt
我希望你能充当一个转译器，将白话转译为我的API能够理解的参数，然后单独返回给我，请只返回参数不要多说别的。
这是规则：
1、如果是播放音乐名或附带歌手（如没有则以歌名结尾），请返回给我：/yun/play/歌名/歌手
2、如果是暂停类似的话，请返回给我：/pause
3、如果是下一首类似的话，请返回给我：/yun/next
4、如果是下一首播放歌曲类似的话，请返回给我：/yun/add/歌名
5、播放歌单，请返回给我：/yun/gedan/歌单名称
6、播放歌单id，请返回给我：/yun/gedanid/歌单名称
7、立即播放音乐id，请返回给我：/yun/playid/歌单id
8、添加指定音乐id到下一首，请返回给我：/yun/add/音乐id
10、播放模式选择【0=顺序播放 1=顺序循环 2=随机 3=循环播放】，请返回给我：/yun/mode/播放模式
```
