---
title: Hexo 建立博客
date: 2018-07-03 16:04:29
tags: [Hexo,前端]
categories: 前端
---

## Hexo 建立个人博客

比较重要的几条命令

### 1.本地测试


``` bash
hexo server
```

### 2.部署到github上


``` bash
hexo deploy -g
```

-g 表示部署在remote之前先生成静态文件


### 3.新建md文件


``` bash
hexo new "article_name"
```

### 4.建tags，categories，about

```
hexo new page tags
hexo new page about
hexo new page categories

```

### 5.怎么插入图片

首先将<font color=red> \_config.yml </font> 中的<font color=red>post\_asset\_folder</font>设为true

然后在根目录下执行
```
npm install https://github.com/CodeFalling/hexo-asset-image --save
```
之后把图片放在和文章名字一样的文件夹下

使用时<font color=red> \!\[logo\]\(文章名/logo.jpg\)</font>

其中[]里面不写文字则图片没有标题

### 6.修改网站图标

将新图标放在/themes/next/source/images

修改next的主题配置文件: \_config.yml

``` bash
favicon:
  small: /images/sheep.png
  medium:/images/sheep.png
```

### 参考资料

https://blog.csdn.net/linshuhe1/article/details/52424573
http://theme-next.iissnan.com/third-party-services.html#swfitype


(gitbash 复制粘贴快捷键：Ctrl+ins/Shift+ins)
