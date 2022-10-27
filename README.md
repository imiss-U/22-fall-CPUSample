# 计算机系统-CPU实验

## 关于同学们能学到什么

- 更加深刻、全面地理解老师课堂上所讲的计算机系统结构知识、CPU的工作过程。相信大家现在对这门课的难度和在它cs专业中的重要性有了一定认知，认真做好实验，不光会锻炼能力，甚至能让你们的期末复习变得轻松。
- 入门一种新的编程语言：`Verilog`。大家可能会觉得搞AI的会`python、cuda`就很了不起了，但是多学点总没坏处。
- 掌握`Linux`平台以及`Git`工具的基础操作。这也会对大家以后的学习、科研或者工作有很大帮助。
- 我们的实验内容基于“龙芯杯”全国大学生系统能力培养大赛，在实验中如果有感兴趣的同学也欢迎联系我，后续有机会可以参加明年的比赛。

## 关于基础需要会什么

考虑到大家的课业安排，我尽可能让大家好上手，以实践课堂所学的理论为主。

实验环境（所需软件和项目包）已经给大家在CG平台准备好，该平台后续也会供你们做Deep Learning相关的项目使用，大家今年有机会提前上手。

`Verilog`作为一门类C语言，相信对大家来说应该不是问题。在实验项目中有部分知识需要大家查阅书籍，相信大三的同学应该也具备不错的自学能力了。

总的来说，实验项目不难，希望大家能够安排好时间，认真对待。

## 关于考核

实验建议2-3人一组，小组评分标准如下（组员分数会以小组分数为基准进行浮动）：

1.功能分 60分（通过`func_test`）

```c++
	10分 pass point 1
        
	10分 pass point 36
	
    10分 pass point 43
	
    10分 pass point 51
	
    10分 pass point 58
	
    10分 pass point 64
```

2.验收分40分（具体分配方式可能会根据同学们的实验情况进行调整）

```c++
	15分 报告
        
	10分 现场测试（加、改代码）
        
	10分 可选模块
        
	5分  github仓库记录
```

2.1 可选模块

```c++
	1.将CPU封装为AXI接口，func_test通过P'64测试点
        
	2.通过P'89测试点
        
	3.通过性能测试，且能够上板验证
        
	4.改进流水线结构，例如六级及以上的流水段，多发射等
        
    5.其它内容（提前联系助教进行评估）
```

还是那句话，实验课程不是为了难为大家，希望大家做完实验后这门课能学得更好。虽然现在看起来任务量不少，但是大家动手认真做就能获得不错的成绩。

如果有同学主动把培养能力的机会全部交给队友，那助教也会在验收时酌情让他的成绩多浮动一些......（助教脾气好，但是不好骗，这项要求是底线）

## 关于后续安排

虽然课表安排的实验课在十二月份，但是考虑到项目工作量，希望大家可以今早开始，为期末周的自己多着想。

### 11.5之前要做的事：

- 组队，和队友协商分工

- 登录自己的CG平台，熟悉服务器环境

- 准备团队的GitHub仓库，学习git基础

- 入门`Verilog`语言，完成一个小任务
### Tips：

#### 1.CG平台服务器的使用

同学们登录自己的CG平台，在课程里面找到`计算机系统`->`在线实验`->`任务一  开始实验`->带有GUI的服务器`界面`。

点击`更多`里面可以选择交互操作，注意服务器装不了中文，每天0点时除了`/mnt/cgshare`目录外，其它位置会恢复为初始镜像状态。因此建议大家在工作结束后及时将代码上传或是下载到自己的电脑。

| 重新连接桌面 | 和浏览器刷新页面一样，如果分辨率卡死或者桌面卡住可以先考虑这个方法 |
| ------------ | ------------------------------------------------------------ |
| 剪切板       | 和本地电脑的剪切操作都需要通过这个中转                       |
| 下载文件     | 下载`cgshare`目录下的文件，文件夹要打压缩包，强烈建议把代码在本地存一份 |
| 上传文件     | 上传内容到`cgshare`目录，小于128M，文件夹要打压缩包          |
| 重新启动     | 和电脑的重启一样，没保存的代码修改会丢失，但是不会清理文件   |
| 桌面还原     | 还原到初始镜像状态，慎点，除非把文件系统搞坏了               |

软件环境已经准备好，还有需要相关的Linux操作大家自行百度。遇见服务器问题解决不了私聊我就好。

#### 2.Git仓库管理

这里推荐大家用`GitHub`，也是以后工作流中的主力，访问方法和创建账户大家自行解决，同学们可以互帮互助一下，要求每个同学都有自己的账户。每个组以`organization`的形式搭建自己的实验仓库，或者在组长的仓库维护自己的分支，虽然需要一定的学习成本，但是习惯了以后要比你们`qq`压缩包日期命名发来发去方便得多。里面的commit记录也会一定程度影响大家的验收分数。（[关于git命令点我看教程](https://www.bilibili.com/video/BV19e4y1q7JJ/?spm_id_from=333.999.0.0&vd_source=fbab33d33705f6c6388c02ca694beb3c)）

大家在初次使用时很容易切错`branch`而导致一天白干，所以建议大家代码在本地保存一份（别放在git的目录下）。

#### 3.Verilog语言入门

大家已经有`c、c++`的基础，参看这篇[教程](https://www.runoob.com/w3cnote/verilog-tutorial.html)就可以快速入门。

我们使用的仿真环境为`Vivado 2019.2`，简单教程放在附录。

服务器上为大家预装了`VSCode`以及`Verilog`相关的插件，如果语法有错误，在`Ctrl+S`后会红线高亮提示，解决完语法问题再开始仿真。

下面是一个小任务，需要以小组为单位，11月5号之前发给助教验收。有不懂的欢迎随时私聊助教，也可以在群里讨论，这样有助于你们后面的工作。

任务程序的Github地址：
