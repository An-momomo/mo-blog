# 关于Liunx的学习（frank）


### 系统
简单来说就是能让我用鼠标和键盘点来点去并且能好我交互让我做一些事甚至能让我安装一些东西的东西。
      PS：没有系统开机只能看到电脑图标

### 世界上目前流行的电脑系统:
- Windows——微软——比尔盖茨
- Linux——林纳斯·托瓦斯创造
      PS:严格来说，liunx是单指操系统的内核
- Unix(Linux的爸爸)——20世纪七十年代于贝尔实验室开发——由C语言创始人创造

开放源代码(开源):我写的代码我公开 公众于世界 集思广益 非商业性
      PS:安卓系统(手机)也是开源的，其核心为Linux。小米、OPPO、vivo、华为……也是由安卓系统改编来的，so我们经常能在手机上看到“基于Android xxx的xx”意味基于安卓系统改编的。安卓系统原版是Google Pixel系列，不在中国内地销售，不支持中国的网络。
      PPS:开源不一定免费

基于Linux的产品:Ubuntu、CentOS、Red Hat、Kali……

## 步入Linux的世界
注：Linux入门不是学“Linux”
体验：比较和其他系统的不同点和相同点
Linux GUI→Shell
Shell↓
右键屏幕
选择Open in Terminal
上图黑框即是


### Linux操作系统：
四个部分
- Linux kernel内核
- GNU工具
- GUI Desktop环境
- Application应用

### Linux内核：
- 硬件设备   管理使用
- 软件程序（系统）——操作软件
- 系统内存
- 文件管理   保存文件，删除文件，修改文件……

### 文件系统：读、写的标准

- GNU：一个组织
- Unix上具有的一些软件，Linux内核本身没有，所以GNU他们模仿Unix，为Linux写了一些必要的软件
- GNU核心：原本在Unix上的一些命令和工具，被模仿（移植）到了Linux上。供Linux使用的这套工具：coreutils coreutilities软件包
       ⑴用来处理文件的工具
         ⑵用来操作文件的工具
         ⑶用来管理进程的工具
  shell提供给用户使用的软件：用户拿它来使用电脑，并和电脑交互
      命令行壳层提供一个命令行界面（CLI）;
      图形壳层提供一个图形用户界面（GUI）
      Linux shell→CLI Command-Line Interface

CLI shell（bash shell基础shell）
右键桌面→进入命令
~/Desktop→在桌面上



其他shell：zsh、ash、korn

GUI：桌面样式
X Windows
KDE
GNOME
Unity

上述为发展史




### shell命令（Linux一切皆文件）
输入命令→执行
 用户名  @  计算机名  在  桌面   [时间]

~ →用户目录/当前所在目录
$ →等待用户输入



### 常见命令

可搜索“Linux命令查询”网站

- ls→显示当前目录下的文件夹和文件（不包括隐藏文件，此时用ls -a）

- ll（ls - list directory contents）→显示文件、用户、时间、形式

- man ** （命令）→显示**（命令）的用法

- cd→打开**（目录）

- cd ..→返回上一级

- /→根目录（Linux最根本的目录）

- pwd→显示当前目录

- gedit  ** （目录）→打开**目录

- touch ** → 创建一个叫 **的文件

- cp ** （想复制文件or文件夹） ** （想复制到的文件）→复制 ** 到 ** [如果复制文件到另一个文件，会使另一个文件被覆盖]

- mv **  ** →移动/重命名 ** 到 **

- 上下键→切换上一个or下一个命令

- &&→并且（可连接两个命令）

- rm→删除文件（rm -f→强制删除）

- sudo rm ~rf /*→删除根目录

- mkdir（make directories）→创建文件夹（mkdir -p→创建一个包含子目录的目录）

- file→查询文件格式

- cat→查看文件（适用于比较短的文件）

- more→以全屏的方式展现（b键→上一页，空格→下一页，q键→退出，回车→下一行）

- less→查看文件

- tail→在屏幕上显示指定文件的末尾几行（tail -n 数字→查看后两行）

- head→在屏幕上显示指定文件的前几行（head -n 数字→查看前几行）

- top→显示或管理执行中的程序ps→显示当前运行的进程

- ps→显示当前运行的进程

- kill→强制结束命令

- df→查看当前所有挂载情况

- mount→改变挂载目录

- du→判断磁盘空间

- sort→对文件内容排序

- grep→搜索文件

- gzrp -h→压缩工具

- tar→压缩工具

- sleep ** （数字）→让终端睡眠** 秒在执行（sleep **&→可以挂在后台做业）

- jobs→查看挂在后台运行的程序

- vim ** （文件）→打开**（普通模式，插入模式，命令模式，可视化模式）

  - 按i键→进入插入模式

  - 按Esc键→进入普通模式
  - 按:wq键→保存（w保存，q退出
  - 上（K）下（J）左（H）右（J）
  - 按i键→光标位置前面插入
  - 按a键→光标位置后面插入
  - 按o键→直接进入下一行输入
  - 按x键→删除光标所在字符
  - 按dd键（两下d）→删除一整行
  - 按u键→撤销
  - 按dw键→移除当前光标所在往后单词
  - 按b键→跳跃单词首字母
  - 按e键→跳跃单词最后
  - 按w键→跳跃下一个单词的首字母
  - 按shift键→联合操作
  - 按p键→粘贴
  - 按yw键→复制一个单词
  - 按y$键→从当前开始复制到末尾
  - 按v键→选择

### 快捷按键     
- Ctrl＋F→向上一页
- Ctrl＋B→向下一页
- Ctrl＋C→强制退出
- Ctrl＋S→保存
- Ctrl＋L→忽略上面的命令
- Ctrl＋T→使光标前的字母后移
- Ctrl＋U→清理光标前的所有东西
- Ctrl＋K→清理光标后的所有东西
- Ctrl＋左右键→跳单词编辑
- Ctrl＋Shift＋C→复制
- Ctrl＋Shift＋V→粘贴
- tab→自动补全

### “/”根目录：
- bin→二进制目录  GNU工具  自带的命令无法更改   许多用户级
- etc→系统配置文件目录
- home→主目录，显示所有用户目录
- lib→库目录，存放系统应用程序库文件
- lost＋found→断电时损失的文件
- mnt→挂载目录，U盘，挂载→外在的设备和电脑进行链接
- proc→虚拟文件系统or伪文件系统
- run→运行目录
- tmp（temp）→临时目录，放一些临时文件
- var→可变目录，放经常变换的文件
- boot→启动目录，放启动用文件
- dev→设备目录，类似Windows的设备管理器
- media→媒体目录
- opt→可选目录，其他第三方软件
- root→root用户的主目录（相当管理员），一般无权访问，若想访问可使用su命令，或使用sudo rm -rf/*获取管理员权限
- srv→服务目录   本地服务
- usr→用户二进制目录，普通用户使用的GUN目录（usr/bin→可找到自己下载的软件）

FHS→文件层级标准
可在http://www.pathname.com中寻找最新版


cd解析
### 文件目录
- 绝对路径：全部的路径
- 相对路径：不全的路径（一定要设置故事背景前提）
     PS：Linux使用相对路径时最前方要去掉
           “/”
       PPS：使用“.（当前文件夹）”就可以使
               用“/”

### 链接文件
- 符号链接（软连接）→快捷方式→左下角带箭头[原来的文件or文件夹必须存在]
- 硬连接

### Linux中的任务管理器→System Monitor
- processes→进程
- Resources→空间
- File Systems→


“;”在命令中的作用
→可以依次执行命令


### 环境变量
- 系统变量
- 用户变量：用户所在变量

- 全局变量
- 局部变量




### 小火车
- 安装：sudo apt install sl
- 卸载：sudo apt remove sl
