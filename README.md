# BingBulr
当前版本:v0.2.1.3 （2018.2.4）<br /> 
下载地址:项目主页BingBulrVxxx.zip是编译好的安装包。 <br /> 
## 使用方法
* 解压BingBulr到非中文目录，如D:\ <br /> 
* 运行 安装.bat，后运行BingBulr.exe，日后每次开启自启动。 <br /> 
* 需要卸载时，运行 卸载.bat ，删除BingBulr目录即可。 <br /> 
## 功能简介
* 每日自动更换Bing壁纸。壁纸区为JP(v0.2.1.3起不再使用CN)。 <br /> 
* 可根据config.ini配置进行局部模糊。 <br /> 
* Windows7系统下默认开机登录界面壁纸替换，壁纸为前一天的壁纸进行半径为80的高斯模糊。 <br /> 
## Config.ini配置简介
__用记事本编辑时，请关闭自动换行，否则出现无法读取配置的BUG。__ <br /> 
### LoginPic ###
* Statue 为1时表示开启开机登录背景替换。 <br /> 
### PicProcess ###
* BulrNum 为进行模糊的区域，默认为1，即任务栏区域。0为关闭模糊功能。 <br /> 
* BulrZoom01,02,03,04,05 分别表示 模糊区域1 的x1,x2,y1,y2（x1x2为横向起始和终止坐标，并非宽度，y轴依然如此），模糊程度（任务栏默认模糊度40）。 <br /> 
* BulrNum为 1 时，BulrZoom1x 设置有效BulrZoom2x 设置无效，以此类推。 <br /> 
<br /> 

# 更新日志 #
## v0.2.1.3
2018.2.4<br />
更换壁纸获取地址为Bing的日本服务器(为解决政策or速度所导致的质量or效率问题。)。
## v0.2.1.2
2018.01.26<br />
自适应多种分辨率屏幕，以比例放大缩小，中心裁剪的方式。
取消默认配置中的底部任务栏模糊，修改为无模糊区域，即壁纸与bing图片完全一致。
修复了无模糊区域时无法设置壁纸的BUG。
## v0.1.1.3
2018.01.03<br />
修复获取XML配置文件可能获取到历史缓存的BUG。<br />
更改无网络状态下尝试获取XML文件的间隔为3秒，以大幅降低无网络状态下CPU的占用。<br />
## v0.1.1.2
2017.12.04<br />
修复部分Win7设备无法清除缓存的BUG。<br />
<br />
## v0.1.1.1
2017.11.20<br /> 
将win7下登录界面背景进行模糊度为80的高斯模糊。<br /> 
增加自动清除缓存功能，想保存今日壁纸可右击桌面点击 保存壁纸到桌面 ，即可保存今日壁纸。 <br /> 
清晰化安装.bat的命名。 <br /> 
 <br /> 
## v0.1.1.0 
2017.11.19 <br /> 
修正无网络状态下获取jpg错误导致opencv内存异常的BUG。 <br /> 
修正win7系统下登录界面背景超过250kb从而无法正常显示的BUG。 <br /> 
修正win7系统下登录界面背景首次开启失败的BUG。 <br /> 
 <br /> 
## v0.1.0.9 
2017.11.14 <br /> 
更换openCV为高斯模糊的模块，减少开机CPU占用，加快缓存生成的速度。无法支持32位系统。 <br /> 
 <br /> 
## v0.1.0.8 
2017.11.09 <br /> 
更新部分WindowsAPI为新版，再无法支持windowsXP。 <br /> 
 <br />  <br /> 
# 源码说明
使用VS2017编写，使用了openCV2.4.13.4和TinyXML开源库，遵循GPL标准。 <br /> 
未使用MFC,MT静态编译。 <br /> 
By Melo@<a href="http://melo.site/">Melo.Site</a> <br /> 
