# Hexo 笔记

## 目录结构
themes
|-主题文件夹
    |-language
    |-layout
        |-_partial
    |-scripts
    |-source
    -_config.yml 

## layout.ejs 
在layout文件夹里，有layout.ejs 文件，提供了基本的目录结构。所有的页面都要依据此页面，并且在body的部分加载不同的地方。<%- body %> 可以加载主页 内容页 甚至正文的内容。都会自动加载到body标签里。加载别的部分。<%- partial('_partial/head') %> 也可以传参。
<%- partial('_partial/mobile-nav', null, {cache: !config.relative_link}) %>

在主题配置文件写的任何内容，可以通过 theme.变量名 访问到

