# Library-Management-System-cpp
使用c++语言，基于动态链表的图书管理系统

> 小白来Github逛逛的第二天

#### 项目文件说明
* SystemBasic基类，为Book和Lend提供系统功能
* Book书籍类，用于存储书籍信息。Lend借阅信息类，用于存储借阅信息
* LibraryProgram.cpp : 此文件包含 "main" 函数。程序执行将在此处开始并结束。

#### 系统简介
* 屎山代码用来丢人
* 支持文件读写
* 链表支持
* 彩色字体
* 修复模式（赚钱用的）
* 光标隐藏
* 管理员用户更改
* 系统时间
* 又编不出来了

#### 项目背景
* 没啥背景单纯用来应付下学校的期末作业（流汗）

#### 更新日志
10-11-2022：第一版
10-11-2022: 类的总体设计:    请参见"/src/Book.svg"和"/src/Book.md"
10-11-2022: SystemBasic:    添加了SystemBasic类并设计了大量方法用于继承与使用
10-11-2022: Book:           添加了Book类并设计了大量方法用于主要的数据与方法
10-11-2022：Book:           添加了管理员登录功能与界面
10-11-2022：SystemBasic:    添加了输入密码时的密码隐藏功能
10-11-2022：SystemBasic:    修复了部分界面排版出错的问题
10-11-2022：SystemBasic:    添加了操作判断：输入n/y yes以继续
10-11-2022：SystemBasic:    修复了缓冲区溢出导致系统无法正常退出的问题
10-11-2022：SystemBasic:    添加了数字合法性的方法
10-11-2022：SystemBasic:    添加了判断失误次数的方法
11-11-2022：Book:           修复了bookData.txt无法读取的问题
11-11-2022：Book:           添加了图书价格合法性的判断
11-11-2022：Book:           添加了在图书查看页面图书库存的判断
11-11-2022：Book:           修复了图书查看页面的借出状态错误的问题
11-11-2022：SystemBasic:    修复了重新进入系统时书籍仓库丢失的问题
11-11-2022：SystemBasic:    添加了无bookData.txt的修复功能
11-11-2022：Book:           添加了在添加书籍时图书ISBN编号的判断功能
11-11-2022：Book:           修复了在添加图书时，图书价格不合法却无法判断的问题
11-11-2022: Book:           添加了删除全部书籍的功能
11-11-2022: SystemBasic:    添加了彩色字体
11-11-2022: SystemBasic:    添加了蓝屏和修复模式 :-)
11-11-2022: SystemBasic:    修改了bookData.txt的修复界面
12-11-2022：SystemBasic:    修复了在蓝屏时进度条超出100%的问题
12-11-2022：SystemBasic:    添加了用于获取系统时间的方法
12-11-2022：Book:           设置了用户借阅时自动填写借阅时间

12-11-2022: 第二版
12-11-2022: Lend:           添加了Lend类用于储存用户借阅信息
12-11-2022: Book:           添加了数据中lendHead指针用于指向第一个Lend类数据以显示借阅信息
12-11-2022: Book:           修复了无藏书时也能修改书籍信息的问题
12-11-2022: Book:           修复了部分界面无法退出的问题
12-11-2022: Lend:           修复了部分排版
12-11-2022: Book:           添加了Lend中信息的文件读写操作
12-11-2022: Book:           修复了Lend中信息的文件读写错误导致数据丢失的问题
12-11-2022: SystemBasic:    添加了获取系统时间方法的模式
12-11-2022: SystemBasic:    解决了由于菱形继承导致的方法冲突
12-11-2022: Book:           删除了Book中部分弃用数据：lendUserId,lendUserName,lendTime
12-11-2022: main:           添加了主界面
12-11-2022: SystemBasic:    添加了主界面显示系统时间
13-11-2022: SystemBasic:    添加了鼠标光标的隐藏和显示功能，并将其运用在蓝屏界面
13-11-2022: Book:           修改文件保存方式，剔除冗余数据
13-11-2022: Book & Lend:    剔除全部无用的注释代码
13-11-2022: SystemBasic:    添加了管理员修改管理员用户的功能
13-11-2022: Book:           修复了管理员修改的数据无法保存的问题
13-11-2022: main:           添加了预加载界面
14-11-2022: main:           添加了预加载界面的加载图 :-)
14-11-2022: Book:           修改了Book中部分情况无法退出、意外退出的问题
14-11-2022: Lend:           修改了next指针的权限（摆烂了）
14-11-2022: main:           添加了主界面的作品信息

14-11-2022: 第三版
14-11-2022: all:            修复了大量界面中异常退出的问题

#### 系统详解
<img width="1154" alt="Book" src="https://user-images.githubusercontent.com/95990919/209258097-4f0fb0a4-06a3-43ac-8e2f-6c9eb3cb7a9a.png">
![IS1T JPPEGG)@9{C7$~~4O4](https://user-images.githubusercontent.com/95990919/209258182-8295695d-08aa-48dd-867b-13679e4f3ff6.jpg)
![流程图](https://user-images.githubusercontent.com/95990919/209258284-0b153a7e-f9d3-4b99-b645-3321c7f5de78.png)
![类图](https://user-images.githubusercontent.com/95990919/209258301-8ce95d23-8d8f-4364-bab8-acba66d3c5b5.jpg)
![图书管理系统](https://user-images.githubusercontent.com/95990919/209258402-7f88e4e3-4ed7-499f-855f-e5f1bf5bd67f.png)


#### 系统截图
![image](https://user-images.githubusercontent.com/95990919/209257740-bd1a92ac-290d-4a93-9c46-7a13bf2d50d8.png)
![image](https://user-images.githubusercontent.com/95990919/209257756-4604eedb-18ac-44f7-9ad4-f1164cb2660e.png)
![image](https://user-images.githubusercontent.com/95990919/209257789-5bdca6b6-d0db-4add-b09c-c0f52f9404cd.png)
![image](https://user-images.githubusercontent.com/95990919/209257834-a90a511a-f018-41c9-af64-21159ef15ecc.png)