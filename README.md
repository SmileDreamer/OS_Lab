    本项目为从零开始做操作系统，前期为纯汇编 nasm 实现，后期采用 tasm + C 实现。

    Lab 01
    设计一个引导扇区程序，程序功能是：用字符‘A’从屏幕左边某行位置45度角下斜射出，保持一个可观察的
    适当速度直线运动，碰到下边后反射，如此类推，不断运动

    Lab 02
    设计满足下列要求的原型操作系统：
    
    1．用户程序大小不等，但最大不超过5个扇区。
    
    2．允许用控制台命令指定一组要执行的用户程序。比如，磁盘上有3个用户程序，可以用命令指定按某顺序
    运行其中1个、2个或3个程序。
    
    Lab 03
    设计满足下列要求的原型操作系统：
    
    (1)用引导程序加载的MYOS内核
    
    (2)内核由汇编语言kernal.asm和c语言kernal.c二个模块生成；
    
    (3)实现作业控制语言mJCB，原型操作系统在当前行显示一个指示符(可以是简单的一个字符或你的学号之类),
    允许用户输入一行命令（回车结束，语法由你设计），操作系统解释命令并完成相应的功能(3个以上的内置
	功能，如time、date、asc等，而且能执行软盘上的某个用户程序)。 

	Lab 04
	设计满足下列要求的原型操作系统：
	(1)操作系统工作期间，在屏幕24行79列位置轮流显示’|’、’/’和’\’，适当控制显示速度，以方便
	观察效果。

	(2)用户程序运行时，键盘事件有事反应：当键盘有按键时，屏幕适当位置显示”OUCH! OUCH!”。

	(3)在内核中，对33号、34号、35号和36号中断编写中断服务程序，程序服务是分别在屏幕1/4区域内显示
	一些个性化信息。再编写一个汇编语言的程序，利用int 33、int 34、int 35和int 36产生中断调用你这
	4个服务程序。

	Lab 05
	改进你的原型操作系统，满足下列要求：

	(1)参考下面的系统调用功能表，增加3个其他功能

	(2)扩展MYOS内核，实现上表中的所有(包括你增加的)系统调用；

	(3)设计C程序库，实现系统调用的封装，并开发一个测试系统调用所有功能的C程序。

	Lab 06
	保留原型原有特征的基础上，设计满足下列要求的新原型操作系统：

	(1) 在c程序中定义进程表，进程数量最多4个。 

	(2) 内核一次性加载4个用户程序运行时，采用时间片轮转调度进程运行，用户程序的输出各占1/4屏幕
	区域，信息输出有动感，以便观察程序是否在执行。 

	(3) 在原型中保证原有的系统调用服务可用。再编写4个用户程序，展示系统调用服务还能工作。

	Lab 07
	原型保留原有特征的基础上，设计满足下列要求的新原型操作系统：

	(1)实现fork()、wait()和exit()。

	(2)内核实现上面三系统调用，并在c库中封装相关的系统调用.

	(3)编写一个c语言程序，实现多进程合作的应用程序。

	可以在下面的基础上完成：一个简单的应用程序例，父进程生成一个字符串，交给子进程统计其中字母的
	个数，然后在父进程中输出这一统计结果。

	Lab 08
	原型保留原有特征的基础上，设计满足下列要求的新原型操作系统：

	(1) 实现信号量机制。

	(2) 内核实现信号量机制后，在c库中封装相关的系统调用.

	(3) 编写一个c语言程序，实现有限缓冲的生产者－消费者模型的应用程序。

	编译连接你编写的用户程序，产生一个com文件，放进程原型操作系统映像盘中。
	
	Lab 09
	原型保留原有特征的基础上，设计满足下列要求的新原型操作系统：

	(1) 映像文件满足FAT12格式。

	(2) 内核以文件形式存放在映像的FAT12文件系统中，修改引导程序实现内核的加载.

	(3) 将所有测试的用户程序放在在映像文件中的FAT12文件系统中，修改内核，实现从文件系统加载
	用户程序。







	
