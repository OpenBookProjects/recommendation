# 推荐序: Django企业开发实战
> Zoom.Quiet  v181119.1824 

## 缘起
突然收到作者邮件邀请来写新书推荐序, 之前对 `the5fire` 这个 ID  并没什么印象.
老规矩,加微信一叙旧才知,居然是6年前会课结下的善缘:
[BPUG-2018-06-09小记 | the5fire的技术博客](https://www.the5fire.com/957.html)

BPUG(北京 Python 用户组)是 04年成立 CPUG(中国 Python 用户组)的北京分会,
从04到07年组织有25次线下会课, 笔者发起并主持了其中绝大多数线下交流活动,
而全国也分别成立了各地城市 Python 用户组, 也不定期组织线下技术交流活动,
至今已进行了总计 50 多场 Python 相关技术交流活动,
作者就是参加了12年那次 BPUG 会课活动后, 坚定了从 JAVA 转变为一名 Pythonic 行者的决心, 进而积累成本书.
参考: [BpugClassesZip - Woodpecker Wiki for CPUG](https://wiki.woodpecker.org.cn/moin/BpugClassesZip)

## 背景
参考: [ PCS304 Python Web应用框架纵论 ](https://wiki.woodpecker.org.cn/moin/ObpLovelyPython/PCS304) 早在 09 年出版的 可爱的Python 一书中, 笔者就对纷繁的 Python web 应用框架进行了讨论. 那之后, 有关 Django 的中文图书并不多, 从 z.cn 上也只查到5本.

但 Django 从05年发布以来, 一直是最活跃以及发展最好的 web 框架社区了,
毕竟一开始就是有对应商业公司支持, 而且基金会一直健康发展.

进而, 在其它大型框架逐渐不活跃后, Django 以其绝对丰富的产品线以及生态环境,成为 Python 世界中商业网站开发的首选框架;

但是, 为何对应图书出版这么不活跃?

答案可能很囧: 因为 Django 官方文档太完备了, 几乎一切应用问题从文档中都可以自行解决, 几乎没有什么特殊知识点需要用图书来解决.
进一步的, Django 社区也极其活跃和友好, 甚至于针对想入门的妹子们, 都有对应的
`Django Girls` 国际品牌活动, 每年组织上千场全天免费培训活动来吸引有一定基础的程序媛从其它技术栈迁移进 Django 世界 ;-)
(对了, 在 PyCon 大会上, Guido 老爹还专门点名赞扬了这一针对萌妹子服务的技术活动)

## 内容
作者绝对是用心的, 其宗旨:

    降低学习 Django 时的心智负担

图书立意明确, 全部代码和经验又全出自真实的项目经历,
之前又正好是作任何事儿先配置N 个 XML 的 SSH 体系忍受者,
自然对 Django "轻巧" 的体系非常热诚, 问题在:

> ...主要是针对想学习Django，但又无从下手，或者看了很久文档，能完成新手教程，但想自己开发一套系统时，却无从开始的人


- 并没有解决 "…但又无从下手" 的根本问题
- 虽然描述了各种叹服的 Django 特性
- 也尝试通过项目的整体概念/流程来引导组织实战工程
- 但是, 所有经验的描述都是以最终成品状态来呈现的,
- 这对有经验的工程师来说可以对比自己的代码来加以理解
- 但是, 对于一开始的目标读者: 无 Django 经验的自学者
- 那就非常困难了...因为我们无法向盲人合理描述明白什么是酱红色吧.

比如, 在正式进行 blog 构建前, 用了⅓ 强的篇幅详细阐述了 Django 商用工程的前期筹备,
以及技术栈介绍, 读者要穿过:
PM/UML/WSGI/Flask/Tornado/DBA/IDE/virtualenv/…
等等一系列成熟技术体系后, 才真正开始构建 blog 原型, 
对于有经验的开发者, 有足够自信可以跳读只印证自己有问题的章节,
对于 Django 初学者就比较苦了.

进而因为篇幅所限, 在 DevOps 进程中, 隐隐涉及到更多工程经验也都没有展开讨论,比如:

- Model 在多人团队中的变更以及管理流程?
- SQLite/MySQL 在协同中的协同/配置/策略?
- Model 在运营中为响应业务变更的升级策略/流程?
- Django 1.x/2.x/django-rest-framework 的选择?兼容?迁移?
- …

## 分析
其实 `降低学习 XXX 时的心智负担` 这类通用解决方案是有的,
就是每一位独立自学成功的开发者都具备的习惯:

- MVP -> 最小可用作品为核心的持续迭代
- 即, 在第一个42分钟, 就完成构建并发布一个几乎没有功能但是, 可运行的 Django 网站
- 然后, 持续迭代, 在一直可运行的基础上, 一点点儿追加功能
- 在这个过程中, 保持 开发/调试/部署/运营 的循环过程
- 确保任何一个新知识点, 立即并入运行中的功能网站
- 这样依据一个健康的开发过程持续积累知识树
- 同时, 有可视/可用/可发布/可演示/可追踪/…活的真实项目来印证

当然, 这样一来, 整个图书的结构, 就不得不包含大量的重复叙述,
无法形成流畅的阅读体验;
所以, 期待作者能用以上这种实战自学过程为线索的思路
(这也是 08 年度笔者提出的 `PythoniCamp` 自学模型), 专门构建一门面向初学者友好的课程.
配合这本其实面向有工程经验者更加友好的图书, 形成 Django 实效系列图书/课程.

## 推荐
综上, 作者从大学时代开始, 独自挣扎了近10年, 终于通过个人努力完成赛道升级, 进入更大的平台 ,开始更强技术的求索, 
本书, 是名靠谱工程师的私人经验集成,
虽然结构和内容上并不完美, 但是, 作者通过样例仓库/私人 blog/公众号 等等渠道,
一直在线, 能持续交流的, 本书的内容也将随着读者的加入持续增订, 
慢慢变成 Django 世界中最可靠的企业工程入门资料库是可以期待的 ;
那么购买本书就成为加入这一丰饶世界的门票了 ;-) 

