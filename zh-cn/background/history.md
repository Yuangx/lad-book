# Linux 历史概述

Linux 是一种自由和开放源代码的类 UNIX 操作系统。也是目前运用领域最广泛、使用人数最多的操作系统。该操作系统的内核由 Linus Torvalds（林纳斯·托瓦兹）在 1991 年 10 月 5 日首次发布。

Linux 最初是作为支持英特尔 X86 架构的个人电脑的一个自由操作系统。目前 Linux 已经被移植到更多的计算机硬件平台，远远超出其他任何操作系统。Linux 可以运行在服务器和其他大型平台之上，如大型主机和超级计算机。Linux 也广泛应用在嵌入式系统上，如手机、平板电脑、路由器、电视和电子游戏机等。

## Unix 的发展历史

1969 年肯·汤普逊(Ken Thompson)在参与美国 AT&T 公司贝尔实验室的 Multics 操作系统项目的过程中开发了一款游戏——《星际旅行》。这是一款飞行模拟游戏。玩家需要控制太空飞船在黑色背景和白色线条组成的太阳系中飞行，并在不同行星和卫星之间着陆，没有特定的目标。

![星际旅行][1]

Multics 项目失败之后，为了能够在 GECOS 系统上继续玩这款游戏，他用 Fortran 语言重写了游戏代码。这款包含许多物理学知识的游戏成功的吸引了包括　Ravi Sethi　和 丹尼斯·里奇(Dennis Ritchie)等人的兴趣。在那个年代，玩游戏可谓代价高昂。因为贝尔实验室内多个终端连接一台中央电脑，终端只有输入/输出的功能，没有运算能力，每个终端要将任务提交到任务队列中，依次排队运行。一旦运行游戏，将会占用很长时间，其他任务只能暂停。所以，玩一次游戏的成本大约是 50 至 75 美元。后来汤普逊发现周围的部门有一台老旧且很少被使用的 PDP-7 小型机，于是又将游戏移植到新系统，但他发现游戏在新机器下运行很慢，于是又吸取了丹尼斯·里奇(Dennis Ritchie)和 Rudd Cassaway 在开发 Multics 文件系统时的经验，在他们工作的基础上设计了自己的文件系统。后经扩展，形成了一个完备的操作系统，在公司内部广泛传播，并于 1970 年被命名为 Unix。

![肯·汤普逊和丹尼斯·里奇一起在 PDP-11 上工作][2]

1973 年，Unix 被丹尼斯·里奇用 C 语言（内核和 I/O 除外）重新编写。高级语言编写的操作系统具有更佳的兼容性，也能更容易地移植到不同的计算机平台。

由于 Unix 的高度可移植性、强大的效能、简洁的系统设计、开放的源代码等特点，吸引了许多其他组织和团体对其进行了扩展，最著名当属加州伯克利分校。他们推出了 Berkeley Software Distributions（BSD）。BSD 系统的主要特性包括： vi 文本编辑器 (ex 可视模式) 、C shell 和 TCP/IP 的早期实现版等，这些特性至今仍被沿用。此外，很多商业公司开始了 Unix 操作系统的衍生开发，例如 AT&T 自家的 System V、IBM 的 AIX 以及 HP 与 DEC 等公司，都有推出自家的主机搭配自己的类 Unix 操作系统。但是，每家公司推出的硬件架构不同，加上当时没有所谓的协议的概念，导致开发出来的 Unix 操作系统以及内含的相关软件并没有办法在其他的硬件架构下工作！1979 年，AT&T 推出 System V 第七版 Unix 后，这个情况就有点改善了。 这一版最重要的特色是可以支持 X86 架构的个人计算机系统，也就是说 System V 可以在个人计算机上面安装与运作了。

![Unix系统衍生简谱][3]

由于商业的考虑，以及在当时现实环境下的思考， AT&T 在 1979 年发行的 System V 第七版 Unix 中，特别提到了『不可对学生提供源代码』的严格限制！同时，也造成 Unix 业界之间的紧张气氛，并且也引爆了很多的商业纠纷。

## MINIX 操作系统

由于 1979 年的版权声明的影响，在大学中不能使用Unix源代码用于教学，促使 Andrew Tanenbaum （谭宁邦）教授自己动手开始编写用于教育用途的 Minix 这个类 Unix 的核心程序。在撰写的过程中，为了避免版权纠纷，谭宁邦完全不看 Unix 核心原代码！并且强调他编写的 Minix 系统与 Unix 系统兼容！到 1986 年 Minix 开发工作终于完成。Minix 并不是完全免费的，无法在网络上提供下载，必须要通过磁盘购买才行，所以 Minix 的传递速度并没有很快速！此外，购买时，随磁盘还会附上 Minix 的源代码！

Minix 除启动部分使用汇编语言编写外，其余部分都采用 C 语言编写。共约 12000 行代码，并作为示例放置在他的著作《操作系统：设计与实现》一书的附录当中。值得一提的是，2015 年之后发布的英特尔芯片都在内部都运行着 MINIX 3，作为 Intel 管理引擎(Intel Management Engine)的组件。

## GNU 计划

GNU 计划，是一个自由软件集体协作项目。1983 年 9 月 27 日由 Richard Mathew Stallman（理查德·斯托曼）在麻省理工学院公开发起。它的目标是创建一套完全自由的操作系统。GNU 是 “GNU is Not Unix” 的递归缩写。

![GNU 计划的标志][4]

到了1985年，为了避免GNU所开发的自由软件被其他人所利用而成为专利软件， 所以他与律师草拟了有名的通用公共许可证(General Public License, GPL)， 并且称呼为 copyleft (相对于专利软件的 copyright！)。

GNU 项目开发出许多高质量的免费软件，其中包括有名的 Emacs 编辑系统、Bash Shell 程序、Gcc 系列编译程序、Gdb 调试程序等等。不过，对于 GNU 的最初构想『建立一个自由的 Unix 操作系统』来说，有这些优秀的程序是仍无法满足的，因为，当时并没有『自由的 Unix 核心』存在。所以这些软件仍只能在那些有专利的 Unix 平台上工作，一直到 Linux 的出现。

## Linux 的发展史

1988 年，Linus Torvalds（林纳斯·托瓦兹）进入了赫尔辛基大学，并选读了计算机科学系。在读期间，接触到了 Unix 系统。当时整个赫尔辛基只有一部最新的 Unix 系统，同时仅提供16个终端（terminal）。早期的计算机仅有主机具有运算功能，terminal 仅负责提供 Input/Output 而已。在这种情况下，实在很难满足托瓦兹的需求，不久之后，他就知道有一个类似 Unix 的系统，并且与 Unix 完全兼容，还可以在 Intel 386 机器上面运行的操作系统——Minix。托瓦兹贷款购买了一台 Intel 386 个人计算机后，便安装了 Minix 操作系统，并通过 Minix 操作系统附带的源代码，学习到了很多内核程序设计的理念。

由 Andrew Tanenbaum（谭宁邦）教授只愿意将 Minix 系统用于教学，不愿意强化系统功能，导致大部分工程师不满足于已有的功能，也使托瓦兹萌生自己编写操作系统的想法。而 GNU 计划产出的 Bash 工作环境和 Gcc 编译程序等自由软件，让托瓦兹能够顺利的编写内核程序。最终，在 1991 年，他写出了能够在 386 计算机上运行的内核，并将其上传到网络上，提供下载。为了让更多 Unix 系统上的软件运行在 Linux 上，托瓦兹参考 POSIX 标准规范修改 Linux，提高了与 Unix 系统的兼容性。

1996年，Torvalds 为 Linux 选定了企鹅作为它的吉祥物。Larry Ewing 提供了吉祥物的初稿。现在正在使用的著名的吉祥物就是基于这份初稿的。James Hughes 根据“Torvalds's Unix”的谐音，取名为 Tux。

![Linux 吉祥物 Tux][5]

## 主要版本

Linux 操作系统从诞生到 1.0 版正式出现，共发布了下表中所示的一些主要版本（引用自《Linux内核完全剖析》赵炯编著的第五页）。

| 版本号 | 发布/编制日期 | 说明 |
| -- | -- | -- |
| 0.00   |   1991.2～4   | 两个进程，分别在屏幕上显示“AAA...”和“BBB...”（注:没有发布） |
| 0.01   |   1991.9.17   | 第一个正式向外公布的 Linux 内核版本。多线程文件系统、分段和分页内存管理。还不包含软盘驱动程序 |
| 0.02   |   1991.10.5   | 该版本以及 0.03 版是内部版本，目前己经无法找到。特点同上 |
| 0.10   |   1991.10     | 由 Ted Ts'o 发布的 Linux 内核版本。增加了内存分配库函数。在 boot 目录中含有一个把 as86 汇编语法转换成 Gas 汇编语法的脚本程序 |
| 0.12   |   1992.1.15   | 主要增加了数学协处理器的软件模拟程序。增加了作业控制、虚拟控制台、文件符号链接和虚拟内存对换（swapping）功能 |
| 0.95.x （即 0.13） | 1992.3.8 | 加人虚拟文件系统支持，但还是只包含一个 MINIX 文件系统。增加了登录功能。改善了软盘驱动程序和文件系统的性能。改变了硬盘命名和编号方式。原命名方式与 MINIX 系统的相同，此时改成与现在 Linux 系统的相同。支持 CDROM |
| 0.96.x |   1992.5.12   | 开始加人UNIX socket支持。增加了 ext文件系统测试程序。 I驱动程序被正式加人内核。软盘类型自动识别。改善了串行驱动、高速缓冲、内存管理的性能，支持动态链接库，并开始能运行 x· Wind“程序。原汇编语言编制的键盘驱动程序已用 c重写。与0，95内核代码比较有很大的修改
| 0.97.x |   1992.8.1    | 增加了对新的 SCSI 驱动程序的支持；动态高速缓冲功能；msdos 和 ext 文件系统支持；总线鼠标驱动程序。内核被映射到线性地址 3GB 开始处 |
| 0.98.x |   1992.9.28   | 改善对 TCP/IP（0.8.1）网络的支持，纠正了 extfs 的错误。重写了内存管理部分（mm），每个进程有 4GB 逻辑地址空间（内核占用 1GB）。从 0.98.4 开始每个进程可同时打开 256 个文件（原来是32个），并且进程的内核堆栈独立使用一个内存页面 |
| 0.99.x |   1992.12.13  | 重新设计进程对内存的使用分配，每个进程有 4GB 线性空间 |
| 1.0    |   1994.3.14   | 第一个正式版本 |


## Linux的核心版本命名

目前最新的内核版本是 2017 年 11 月 24 日公布的 4.14.2 版，Linux 内核版本号命名的规则：r.x.y
* r：表示目前发布的内核主版本。
* x：x是偶数表示稳定版本，主要用于企业等生产环境; 若是奇数表示开发中版本，主要用于开发和测试新功能。
* y: 修订版本号，表示修改的次数。

## 名称争议

GNU 计划的支持者与开发者，特别是其创立者 Richard Matthew Stallman（理查德·斯托曼）主张 Linux 应称为“GNU/Linux”较为恰当，因为此类操作系统使用了众多 GNU 程序，包含Bash（Shell 程序）、库、编译器等等作为 Linux 内核上的系统包。Linux 社区中的一些成员，如Eric Steven Raymond（埃里克·斯蒂芬·雷蒙）、Linus等人，偏好 Linux 的名称，认为 Linux 朗朗上口，短而好记，拒绝使用“GNU/Linux”作为操作系统名称。并且认为 Linux 并不属于 GNU 计划的一部分。现在，有部分 Linux 发行版，如 Debian ，采用了“GNU/Linux”的称呼。


## 参考资料

- Linux 内核完全剖析[M],赵炯,机械工业出版社,2016
- Linux 内核设计的艺术:图解 Linux 操作系统架构设计与实现原理[M],新设计团队,机械工业出版社,2013
- 鸟哥的 Linux 私房菜 基础学习篇[M],鸟哥,人民邮电出版社,2010
- Linux EB/OL, https://zh.wikipedia.org/zh-cn/Linux
- Space Travel EB/OL, https://zh.wikipedia.org/wiki/%E6%98%9F%E9%99%85%E6%97%85%E8%A1%8C_(1969%E5%B9%B4%E6%B8%B8%E6%88%8F)
- BSD EB/OL, https://zh.wikipedia.org/zh-cn/BSD
- Minix EB/OL, https://zh.wikipedia.org/zh-cn/Minix
- History_of_Linux EB/OLx, https://en.wikipedia.org/wiki/History_of_Linux 

  [1]: https://upload.wikimedia.org/wikipedia/commons/4/46/Space_Travel_Screenshot.png
  [2]: https://upload.wikimedia.org/wikipedia/commons/thumb/8/8f/Ken_Thompson_%28sitting%29_and_Dennis_Ritchie_at_PDP-11_%282876612463%29.jpg/1024px-Ken_Thompson_%28sitting%29_and_Dennis_Ritchie_at_PDP-11_%282876612463%29.jpg
  [3]: https://upload.wikimedia.org/wikipedia/commons/thumb/7/77/Unix_history-simple.svg/1024px-Unix_history-simple.svg.png
  [4]: https://upload.wikimedia.org/wikipedia/en/thumb/2/22/Heckert_GNU_white.svg/535px-Heckert_GNU_white.svg.png
  [5]: https://upload.wikimedia.org/wikipedia/commons/thumb/3/35/Tux.svg/280px-Tux.svg.png