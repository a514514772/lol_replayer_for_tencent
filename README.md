# lol_replayer_for_tencent 介绍
League Of Legends 英雄联盟，腾讯游戏助手TGP录像的解析代码，可搭建录像服务器，启动游戏进行观看录像。

# 程序实现的技术分析
在mac osx上看lol国服ob录像的技术分析： http://www.cnxct.com/how-to-watch-lol-tencent-ob-on-mac-osx/

#编译
``cfc4n@cnxct:~/Project/github/lol_replayer_for_tencent$go get github.com/collinglass/mw
cfc4n@cnxct:~/Project/github/lol_replayer_for_tencent$go get github.com/gorilla/mux
cfc4n@cnxct:~/Project/github/lol_replayer_for_tencent$go get github.com/pborman/getopt``

cd 项目目录

``cfc4n@cnxct:~/Project/github/lol_replayer_for_tencent$sh shell/build.sh``



#使用：
>在 http://api.pallas.tgp.qq.com/core/get_ob_list 中，有很多http://ob.pallas.tgp.qq.com/ob_data/1_1789151000.ob 字样的录像文件，下载下来

``cfc4n@cnxct:~/Project/github/lol_replayer_for_tencent/bin$./launcher -f  1_1789151000.ob``

#备注
windows平台需要在编译时，填写LOL游戏所在目录

#GUI
我們提供了windows的GUI，請先將launcher編譯完成後放到LoL client資料夾底下，再進入LoL_replayGUI開啟application重播。
(目前仍在建構中，敬請期待)
