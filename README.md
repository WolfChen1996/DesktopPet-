# 《刀刀的猫猫》
**作者：狗头人 www.wolfchen.top**  
**QQ群：<a href="https://jq.qq.com/?_wv=1027&amp;k=uml41LED">980897840</a>** 

## 项目简介
我的好朋友大菜刀很想养一只猫，可是她太菜了，不能养猫，于是我决定做一只给她。  
第一阶段，完成一个能走能跳能睡觉，可抓鼠标会吃图标，点一点它还能在地上打滚的猫猫，现在进度大概50%了。  
第二阶段，希望能做出一个，每个人都可以随便涂涂画画，就能生成自己的专属猫猫的软件。  
第三阶段，是加上一点点社区功能，好友之间可以分享宠物，或者去串门。  
“我的梦想，是让每个人都可以轻松地制作属于自己的桌宠！”  
如果有人想一起监工，或者想帮忙画一点东西，抑或是想做一个自己的宠物，欢迎加qq群讨论   
  
## 计划、进度和开发记录
接下来 
制作设置面板  
优化猫猫动画，增加爬墙动作 
添加2~3个宠物  
创意工坊和模型生成器  
  
  
<table>
<tr><th>	日期	</th><th>	完成事项	</th><th>	新知识	</th></tr>
<tr><td>	2022.02.09	</td><td>	《刀刀的猫猫》正式立项，决定使用Unity制作	</td><td>	Unity里给camera增加代码制作背景透明的效果	</td></tr>
<tr><td>	2022.02.10	</td><td>	决定将制作工具从unity改为python，虽然做起来更难了，但是后续可以增加更多功能，比如吃桌面上的图标。	</td><td>	pyqt5的安装与基础使用	</td></tr>
<tr><td>	2022.02.13	</td><td>	可以正常显示了！	</td><td>	pyqt5全屏显示、背景透明、label以及Qpixmap	</td></tr>
<tr><td>	2022.02.13	</td><td>	Demo制作完成	</td><td>	原来俺真的可以做一个桌宠	</td></tr>
<tr><td>	2022.02.14	</td><td>	吸附底端、自由掉落以及左右移动的功能完成了。开始制作动画以及画猫猫。	</td><td>	QDesktopWidget().screenGeometry()以及QDesktopWidget().availableGeometry()，可以分别获取屏幕尺寸和桌面尺寸（去掉开始菜单）	</td></tr>
<tr><td>	2022.02.15	</td><td>	把猫猫站立姿态的素材处理完了，并绑定了骨骼	</td><td>	复习了AN的骨骼操作	</td></tr>
<tr><td>	2022.02.16	</td><td>	完成了猫猫眨眼的动画，并添加了把猫猫丢来丢去的功能，同时完善了配置文件的使用逻辑，修复了许多bug	</td><td>	写了一个小小的物理引擎，复习了等比数列的相关公式，意识到我的数学是挺菜的。	</td></tr>
<tr><td>	2022.02.16	</td><td>	试图制作快速选择宠物的菜单	</td><td>	学习了qt二级菜单和lambda，但是lambda没啥卵用，不知是有bug还是机制问题，后续将用QButtonGroup尝试	</td></tr>
<tr><td>	2022.02.17	</td><td>	完成了拎起来和掉落的动画，优化了动画播放逻辑	</td><td>	在CC的帮助下，添加了一个类，实现了lambda传参的问题	</td></tr>
<tr><td>	2022.02.18	</td><td>	画了一个走路的猫脑袋。更新了歪脑袋的动作，以及很多你们感觉不到但是我真的做了的细节优化，提升了运行效率和内存占用量	</td><td>	画画的水平得到了轻微的提升	</td></tr>
<tr><td>	2022.02.19	</td><td colspan="2">	休息一天			</td></tr>
<tr><td>	2022.02.20	</td><td  rowspan="6">	"这几天吃不好也睡不好，每天都在想这个猫猫。有很多问题，现有结构是没法实现的，比如mac的适配，开始菜单的置顶，切换宠物之类的功能，因为多套了一层窗口，很多东西想优化却无从下手，所以决定进行一次重构。

经过这几天的努力，完全重构了猫猫，彻底理解了pyqt5的逻辑关系，并确定了今后的项目数据结构。顺手解决了mac的兼容性问题，添加了几个功能和参数，并修复了切换宠物、放大缩小等功能里的bug。"	</td><td  rowspan="6">	"python中遍历目录下的文件并排序
pyqt5在mac中的使用
"	</td></tr>
<tr><td>	2022.02.21					</td></tr>
<tr><td>	2022.02.22					</td></tr>
<tr><td>	2022.02.23					</td></tr>
<tr><td>	2022.02.24					</td></tr>
<tr><td>	2022.02.25					</td></tr>
<tr><td>	2022.02.26	</td><td>	项目结构改动会影响加载速度，需要重新考虑一下，暂时调整回原来的样子	</td><td>	学会了configparser的读写	</td></tr>
<tr><td>	2022.02.27	</td><td colspan="2">	休息一天			</td></tr>
<tr><td>	2022.02.28	</td><td colspan="2">	休息一天			</td></tr>
<tr><td>	2022.03.01	</td><td>	修复bug	</td><td>		</td></tr>
<tr><td>	2022.03.02	</td><td  rowspan="5">	制作了【设置面板】，这样就不用修改配置文件了，方便了许多。	</td><td  rowspan="5">	"学习了qt designer的使用，以及如何导出ui文件，如何添加qrc
学习了emit和QtCore.pyqtSignal，理解了connect的逻辑。
了解了如何把ui文件和qrc文件转成py并导入到项目中去"	</td></tr>
<tr><td>	2022.03.03					</td></tr>
<tr><td>	2022.03.04					</td></tr>
<tr><td>	2022.03.05					</td></tr>
<tr><td>	2022.03.06					</td></tr>
<tr><td>	2022.03.07	</td><td>	修复bug	</td><td>	不要忘记初始化self.is_follow_mouse	</td></tr>
<tr><td>	2022.03.08	</td><td  rowspan="2">	用翻转左走图片，做了临时的右走动画	</td><td  rowspan="2">	学会了如何翻转图片	</td></tr>
<tr><td>	2022.03.09					</td></tr>
</table>  

  
## 使用说明
### 运行：  
windows用户直接双击【pet.exe】就可以运行啦，如果需要多只，多点几次即可。  
辣鸡苹果的用户请查看【mac运行指南.txt】，自己下个python，装几个包，编译运行。后期应该会打包辣鸡mac的app，反正现在是有点bug，还在研究中。

### 修改宠物：  
可直接进入对应文件夹修改图片；如需增减图片，需要修改文件夹中petconfig.ini文件（双击用文本文档打开即可），配置文件内有注释，对着修改每个状态对应的文件名即可。   

### 添加宠物：  
需要在config.ini文件中（右键》编辑，用文本文档打开即可），添加一个宠物的id，并前往data文件夹中添加一个和id对应的文件夹，并添加参数文件（从其他宠物的文件夹复制一个petconfig.ini过来）和图片。  
后期计划制作模型生成器和共享宠物的平台，希望日后可以很方便地创建或下载自己想要的宠物。
  
~~不过设置面板很快就好了，之后就不用去改文件啦。~~
设置面板做好了，修改宠物的话直接在设置面板修改即可。不过添加宠物可能还是要改改配置文件。
  
## 参数说明  
### 【config.ini】
#这是配置文件，如果添加宠物，需要修改下面的petids数组；  
#可以通过修改petid更改默认宠物。  
#可以通过修改traypath修改托盘图标  
[config]  
#宠物id，可以是字母或者汉字，用英文逗号隔开  
petids=1,2,cat1  
#默认宠物的id  
petid=cat1  
#托盘图标路径  
traypath=./data/tray.png  
  
### 【petconfig.ini】
[config]  
#宠物名字  
petname=Black Cat

#宠物缩放等级，1就是原尺寸，0.5就是一半，2就是2倍  
petscale=0.15

#底部偏移距离，可以用来制作一部分爪子露在开始菜单外面的样子。正数往下  
bottomfix=0

#丢来丢去的速度（水平）  
dragspeedx=0.5

#丢来丢去的速度（竖直）  
dragspeedy=0.3

#是否可以往两边扔出去(yes/no)  
throwout=yes

#是否可以往开始菜单里走(yes/no)  
intotray=no

#重力加速度，影响掉落速度  
gravity=4

#刷新速度  
gamespeed=10


#可修改默认动作的图片数量和触发概率。  
#默认动作类型，其中stand,walkleft,walkright,drag,falling，分别对应站立，向左走，向右走和提起，为必备参数，别改。  
petaction=stand,walk,walkright,drag,falling

#走路速度  
petspeed=5

#默认动作的图片个数，文件名为stand1.png，stand2.png~standX.png，到几就写几，到100就写100。分别对应站立，向左走，向右走，提起，掉落  
petactionnum=1,26,1,5,1

#站立和左右走动的占比，0.5代表50%，三个数加起来等于100%；自定义动作包含在站立里  
petactionrate=0.95,0.05,0

#拖拽时坐标偏移，用于改变拖拽时宠物和鼠标的相对位置，比如要拎起脖子之类的。x正数往右，y正数往下。  
dragingfixx=0  
dragingfixy=1000

#以下为自定义动作  
#自定义动作类型  
standaction=stand,blink,shake

#自定义动作的图片个数，文件名为stand1.png，stand2.png~standX.png，到几就写几，到100就写100。要加单引号  
standactionnum=1,12,12

#每种自定义动作播放的占比，0.5代表50%，加起来小等于100%，若不满100%，则显示第一个动作  
standactionrate=0.9,0.05,0.05
  
## 写在最后
本项目由想养猫又养不了的大菜刀独家逼迫狗头人完成  
早期参考了以下两个项目的框架  
https://github.com/Laylar-sleep/DesktopPet  
https://github.com/SpeedPromise/DesktopPet  

## 特别感谢  
xixi提供了切换宠物的代码思路  
Maggie的鼓励  
帮忙找bug的ZZP-DMU  
建议在初始化中添加is_follow_mouse的F  
以及大菜刀的逼迫！  
还有各位小伙伴的支持！  
