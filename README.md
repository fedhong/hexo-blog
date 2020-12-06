# hexo-blog

* hexo init [folder]

新建一个网站。如果没有设置 folder ，Hexo 默认在目前的文件夹建立网站。

* hexo new [layout] <title>

新建一篇文章。如果没有设置 layout 的话，默认使用 _config.yml 中的 default_layout 参数代替。如果标题包含空格的话，请使用引号括起来。 hexo new "post title with whitespace"

-p, --path	自定义新文章的路径

-r, --replace	如果存在同名文章，将其替换

-s, --slug	文章的 Slug，作为新文章的文件名和发布后的 URL

* hexo generate

生成静态文件。该命令可以简写为hexo g

-d, --deploy	文件生成后立即部署网站

-w, --watch	监视文件变动

-b, --bail	生成过程中如果发生任何未处理的异常则抛出异常

-f, --force	强制重新生成文件,Hexo 引入了差分机制，如果 public 目录存在，那么 hexo g 只会重新生成改动的文件。使用该参数的效果接近 hexo clean && hexo generate

-c, --concurrency	最大同时生成文件的数量，默认无限制

* hexo publish [layout] <filename>

发表草稿。

* hexo server

启动服务器。默认情况下，访问网址为： http://localhost:4000/。

-p, --port	重设端口

-s, --static	只使用静态文件

-l, --log	启动日记记录，使用覆盖记录格式

* hexo deploy

部署网站。该命令可以简写为： hexo d

-g, --generate	部署之前预先生成静态文件

* hexo clean

清除缓存文件 (db.json) 和已生成的静态文件 (public)。

在某些情况（尤其是更换主题后），如果发现您对站点的更改无论如何也不生效，您可能需要运行该命令。

* hexo list <type>

列出网站资料。


* 文档

https://hexo.io/zh-cn/docs/commands
 