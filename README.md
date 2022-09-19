# 2022-April-Tour-BE

## 前言

欢迎来到 OverClock 2022 秋招后端组实习仓库

后端相关学习资料已经通过邮件的形式发送给各位师傅了，接下来就是理论落地，生产第一个后端小项目的时候了

- 开发规范
  - 在本仓库中 base main 分支创建属于自己的分支，分支命名方式为：TASK_NAME；例如李元元同学选择实习题目作业收集器（HC）作为自己的实习题目，则命名为：HC_SBY
  - 我们鼓励每写完一个函数或一个服务就进行一键三连以在 github 上能查看你的完整commit记录
  - 建议在自己的分支下替换 README.md 为自己的项目文档，包括但不限于API设计、架构设计、功能实现、每日版本更新情况等（美观的MarkDown文档编写也作为考核指标）
  - 对于敏感信息例如 Config.json 应当使用 .gitignore 避免上传Public仓库
  - 我们鼓励同选题的师傅们相互学习，但请避免直接抄袭，可以借鉴github上其他优质项目

## 选题

选题有难度区分，已经在题目描述中暗示难度差异（请在量力而行的基础上让我看到你的野心hhh）

对于题目描述不理解的地方可以私戳沟通

部分选题中有一些帮助链接，可能因为时效性原因并不一定能复现原文效果，各位师傅应该锻炼自己的信息搜集能力solve这些问题

### 作业收集器 Homework_Collector（HC）

- 项目背景
  - 小董同学上大学以后，为了获得优干奖学金，踊跃报名成为了一名学习委员，没想到这学期有这么多课都要交作业：组原、大雾、危机昏、毛概...，小董同学直接自闭，这学委怎么这么难当啊。热心的你为了帮助你的女神小董，你决定使用你刚学的golang编程实现一个简单的作业收集器来实现作业收集。
- 基础功能
  - 作业收集（用户可以通过访问url或者api接口来实现文件上传）
  - 作业分组（用户上传文件时通过参数指定科目，后端可以将同科目作业放在同一路径下）
- 进阶功能
  - 上线服务器（如果选择进阶则必做，没有服务器可以向团队申请服务器账号和端口）
  - 作业提醒（向后端服务器发送一条带收件人邮件地址列表的请求，后端服务器批量发送邮件提醒该交作业啦）
  - 作业分享（生成一个作业分享链接，B同学通过分享链接可以访问A同学之前上传的作业）
- 高级功能
  - 安全升级（如果选择高级功能需要在答辩前三天联系SBY，不被SBY攻击成功则算完成）

### 我的音乐 My_Music（MM）

- 项目背景
  - 小徐同学是一个深度音乐爱好者，无论做什么她都要带着耳机听音乐。但是她也有个烦恼，就是各大音乐软件的资源存在差异，例如可能存在歌手A的歌只有酷狗有版权，在网抑云就听不了了，由此就造成了小徐同学需要切换不同的软件去听歌，这实在太蓝瘦辣！于是热心的你决定帮助你的女神小徐，使用你已经练习时长一年半的golang编程来实现一个你自己的音乐播放服务。
- 基础功能
  - 音乐爬虫（巧妇难为无米之炊，先去全网爬一些音乐文件⑧）
    - https://www.bilibili.com/video/BV1SA4y1976A?p=23&vd_source=39fee886ab3becb97a63df43730a53e4
    - https://www.cnblogs.com/liuzhongkun/category/2101562.html
  - 歌词爬虫
    - https://blog.csdn.net/weixin_42742658/article/details/103484096
    - https://www.jianshu.com/p/008c99877f30
- 进阶功能
  - 上线服务器（如果选择进阶则必做，没有服务器可以向团队申请服务器账号和端口）（本题目中存在爬虫，请一定注意不要下载太多文件炸掉服务器）
  - 壁纸爬虫（你知道小徐同学是个二刺猿之后，决定专门开发一个爬取好看图片的功能来为你的音乐播放增加一点乐趣，注意小徐同学是个二刺猿，所以请选择合理的网站去爬取）
  - 注册登录（小徐很美，但美丽的花朵是那么的多，作为渣男，你决定让更多人使用这个音乐播放器，所以你允许别人注册登录你的平台）
- 高级功能
  - 考验这个系统的坚挺性，爬了两三首歌就被反爬干掉了是不行的哦

### 华科帮帮忙 HUST_Helper （HH）

- 项目背景
  - 小沈同学是一个小公举，来上大学之后发现身边的大家怎么那么独立呀！每天她希望能有A同学骑车带她上课，B同学给她喂饭，C同学帮她写作业，... 所以她在全校招募技术大佬帮她写一个供需平台发布她的需求帖，本来热心的你对这样的巨婴是很无语的，但是她给的实在太多辣，于是你决定用你练习时长两年半的golang写一个平台来恰钱hhh
- 基础功能
  - 注册登录（你不想平台内混入骗子（不是校友都算骗子），所以只有登录后才能查看平台内容，并且需要验证校园邮箱验证身份）
  - 发布帖子（需求帖）
  - 帖子展示板块（需求帖list）
  - 单项帖细节展示（需求贴detail）
- 进阶功能
  - 需求贴分类（通过不同标签来区分帖子区别，比如交友、卖二手、表白、...）
  - 分类展示（用户通过选择需要的类别来展示更有针对性的帖子）
  - 评论（针对某一帖子进行评论）
- 高级功能
  - 帖子审核（我要是发布一个骂人帖肿么办，不能我想发啥垃圾就发啥吧hhh）

