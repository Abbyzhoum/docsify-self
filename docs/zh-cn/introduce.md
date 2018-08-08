###  此文档是基于Markdown  语法和docsify 文档生成器
>   Markdown现在基本上很多人在用，覆盖面蛮广的，评价✨✨✨

>  如果有文档说明,需求总结之类的可以使用docsify, 评价✨✨

> 前言

这个文档介绍和整理我用过不错的网站的还有大神推荐的,比较适合web前端开发人员(我就是其中一员),另外也可以了解Markdown和docsify语法

> docsify
  一个神奇的文档生成器


 入门教程
  步骤说明：



①  全局安装docsify  
    命令行： yarn global add docsify-cli   yarn安装
                    npm i docsify-cli -g  npm安装

②   初始化  
         docsify init ./docs    初始化 docs文件夹下的所有文件获取环境
        docsify init <path> [--local false] [--theme vue]  使用init生成您的文档
        <path>默认为当前目录。使用像./docs（或docs）这样的相对路径。

* --local 选项：
    * 速记： -l
    * 输入：boolean
    * 默认： false
    * 说明：复制docsify文件的文档路径，默认为false使用unpkg.com作为内容递送网络（CDN）。要显式设置此选项以false使用--no-local。
* --theme 选项：
    * 速记： -t
    * 输入：string
    * 默认： vue
    * 说明：选择一个主题，默认为vue，其他的选择是buble，dark和pure。

③   serve命令
        docsify serve docs     运行本地服务器http://localhost:3000

④   代码片段  
        参照此文档😁😁😁😁😁😁😁😁😁😁

⑤   详情参照官网

       docsify --> https://docsify.js.org/#/
       markdown --> https://github.com/younghz/Markdown
