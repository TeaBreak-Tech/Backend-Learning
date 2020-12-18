# 后端学习


## 圣诞假期任务：

1. **每周**在GitHub上写一周的学习笔记。
2. 在圣诞假期结束前 (deadline: 1.10 24:00)，完成活动日历项目，具体要求如下：
   1. 如这封活动邮件：![活动邮件示例](https://raw.githubusercontent.com/doutv/Picbed/master/img/README-2020-12-18-22-03-53)
   2. 实时接收并识别邮件内容。
   3. 提取活动主题、时间、地点、内容、讲者等信息。
      1. 至少需要提取时间和地点，而活动的其余信息可以以邮件原文的方式展示。
3. 试用期评价方式：
   1. __活动日历__（主要）
      1. 完成度及识别准确率
      2. 代码风格（命名不要太烂就行，注释不要求）
   2. 学习笔记
   3. 其他贡献：
      1. 对已有项目的完善
      2. 对本学习文档的完善

## Week 1 实用工具及技巧

Git和Markdown是必须学习的内容

* Google
    * 学会如何用英语描述问题并在Google上找到答案
        * 95%的问题都可以解决
        * 程序员最应该掌握的语言是英语
        * （不想看英文还有Google翻译）
    * Stack Overflow而不是CSDN
        * 虽然CSDN上也有不少优质内容，但是大部分都是从英文网站翻译过来或者抄袭别的文章
        * 个人认为在中文论坛里面，知乎，简书，Segment Fault不错
* Git
    * Overview
    * Basic commands
        * add
        * commit
        * pull
        * push
    * gitignore
        * [https://www.cnblogs.com/kevingrace/p/5690241.html](https://www.cnblogs.com/kevingrace/p/5690241.html)
    * GitHub
        * Pull Request
        * Issue
        * git clone
        * __加入TeaBreak Team__
            * 在Team下创建一个存放学习笔记的仓库
                * 新建仓库后`git clone`到本地
                * 将本地git仓库推送到GitHub上
                    * `git remote add origin`
                    * `git remote -v`
        * Optional:
            * SSH keys [https://github.com/settings/keys](https://github.com/settings/keys)
            * Explore great repositories
            * Plugin 浏览器扩展
              * Sourcegraph https://about.sourcegraph.com/
    * git图形化界面
        * VsCode
        * git gui
    * 参考
        * [https://missing.csail.mit.edu/2020/version-control/](https://missing.csail.mit.edu/2020/version-control/)
        * [https://learngitbranching.js.org/?locale=zh_CN](https://learngitbranching.js.org/?locale=zh_CN)一个交互式的git教程
* 选IDE
    * VsCode
    * Pycharm
    * etc.
* 掌握Markdown语法
    * 本文档就是用Markdown写的
    * 又简单又美观
    * __用Markdown写学习笔记__
        * 偷偷推荐一下自己的Blog: https://jasonblog.xyz/2020/01/12/2020/1-6/#toc-heading-1
        * Markdown文件`1-6.md`也放在仓库下了
        * 写法仅供参考，爱咋写咋写😄
    * Optional:
        * Markdown转换成pdf
        * Latex数学公式
            * 可以用来写数学作业
* 考虑学习Vim
    * Vim是世界上最好的文本编辑器
    * 但是学习曲线不友好
    * 在大部分IDE中都可以用Vim插件
    * 命令行环境下Vim很好用
    * 甚至在Chrome中也可以用Vim: Vimium实现无鼠标上网
        * [https://www.zhihu.com/question/23483616](https://www.zhihu.com/question/23483616)
        * [https://chrome.google.com/webstore/detail/vimium/dbepggeogbaibhgnhhndojpepiihcmeb](https://chrome.google.com/webstore/detail/vimium/dbepggeogbaibhgnhhndojpepiihcmeb)
    * 参考
        * [https://coolshell.cn/articles/5426.html](https://coolshell.cn/articles/5426.html)
        * [https://missing.csail.mit.edu/2020/editors/](https://missing.csail.mit.edu/2020/editors/)
### Tasks

- 在GitHub上加入TeaBreak Team并创建你的学习笔记仓库
- 用Markdown完成你的第一篇学习笔记

## Week 2 Python语法 & Django入门

### Python语法

官方文档：https://docs.python.org/3/

廖雪峰的python教程：https://www.liaoxuefeng.com/wiki/1016959663602400

+ 数据类型
+ 流程控制
  + 条件判断
  + 循环
+ 函数
+ 数据结构
  + 列表
  + 字典
+ 异常处理
+ 模块和包
  + 以下三种`import`的区别：
    + `import json`
    + `from json import *`
    + `from json import load`
+ 类
  + 类成员
  + 类方法
+ 装饰器（选学）

### Django入门

官方文档：https://docs.djangoproject.com/zh-hans/3.0/

在实践中学习Django会比较快，哪里不会查哪里，首先在官方文档里找，其次用Google搜索。

1. 推荐大家先跟着教程做一个简单的应用：https://docs.djangoproject.com/zh-hans/3.0/intro/tutorial01/
2. 在我们团队中，Django仅作为后端使用，推荐大家阅读问答墙后端代码：https://github.com/TeaBreak-Tech/ciwkbe
   1. 阅读后端README
   2. 数据库增删查改 `QuerySet`
   3. `HttpResponse` 统一定义
   4. 装饰器
      1. `post_token_auth_decorator` 减少冗余代码
      2. `require_http_methods` 指定http method
   5. 欢迎大家来完善后端代码：在微信群里提出建议 -> 新建分支 -> 在新分支上变更 -> Pull Request / 直接合并到master

### Tasks

- 跟着教程做一个简单的Django应用：https://docs.djangoproject.com/zh-hans/3.0/intro/tutorial01/
- 探索问答墙后端代码：https://github.com/TeaBreak-Tech/ciwkbe

## Week 3 搭建项目

难点：自动识别某封邮件是否是活动邮件并提取关键信息

可能的解决方案：

- 多看几封活动邮件试图找到它们的共同点，用`str.find()`或__正则表达式__匹配
  - 正则表达式学习：
    - https://deerchao.cn/tutorials/regex/regex.htm 理论
    - https://regex101.com/  交互式学习，强推
    - https://regexone.com/  几道练习题
- 机器学习相关：自然语言处理NLP？

## Week 4 Linux

学有余力的同学可以继续往下学~

* SSH
    * 原理
    * 如何实现免密登录服务器
* 常用命令
    * 文件
        * 
