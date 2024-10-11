使用luckfox rv1106的sdk开发SoloLinker开发板，现在仅支持了build luch中的8选项，使用spi nand的版本，摄像头支持gc2093和gc4653
# 编译方式
./build.sh lunch
输入8
./build.sh
# Wifi连接方式
1. 插上wifi短接线
2. 等待系统启动到登录打印，此时输入账号名 root 回车后输入密码 luckfox 回车即可进入系统
3. 输入下面两行指令加载wifi驱动
```bash
cd /oem/usr/ko/
./insmod_wifi.sh
```
4. 连接wifi
```bash
wifi_start.sh <SSID> <password>
```
5. 查看设备ip地址
6. 使用vlc打开上面地址的rtsp连接播放
rtsp://192.168.1.5/live/0
