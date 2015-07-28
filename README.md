## 目录

* [任务描述与要求](#任务描述与要求)
    * [描述](#描述)
    * [要求](#要求)
    * [RIA相关学习材料](#相关学习材料)
* [开发文档](#开发文档)
    * [项目结构](#项目结构)

# 任务描述与要求

这个仓库用于完成 [RIA扬帆班任务一：图片网站](https://github.com/baidu-ife/ife/blob/master/2015_summer/task/ria_yangfan_01.md)

## 描述

实现一个个人图片展示网站，包括展现及后台管理。

[设计图](design.md)

## 要求

* 团队协作完成
* 支持在管理端拖拽图片来改变图片的分类，以及图片在展示页面的排列顺序
* 支持在管理端通过拖拽分类来改变分类在展示页面的排序
* 支持在管理端上传图片，上传功能可以使用第三方组件，比如[WebUploader](http://github.com/fex-team/webuploader/)
* 除了jQuery及WebUploader，不允许使用其他框架类库
* 不需要登陆注册等功能
* 如果需要使用Server端，不限制语言，Server端框架使用不限制

## 相关学习材料

* [what is a single page application (Wikipedia)](https://en.wikipedia.org/wiki/Single-page_application)
* [Single page apps in depth](http://singlepageappbook.com/index.html)
* [Important Considerations When Building Single Page Web Apps](http://code.tutsplus.com/tutorials/important-considerations-when-building-single-page-web-apps--net-29356)
* [JavaScript Single Page Application Frameworks](http://stackoverflow.com/questions/14336450/javascript-spa-frameworks-single-page-application)
* [Developing Single Page Apps with Backbone.js](https://singlepagebook.supportbee.com/)
* [AngularJS Tutorial - Building a Web App in 5 minutes](https://www.airpair.com/angularjs/building-angularjs-app-tutorial)
* [Building single page apps using web components](https://www.polymer-project.org/0.5/articles/spa.html)

# 开发文档

* 这里记录开发过程的所有说明、架构、技术选择、工具选择、合作方式等。
* 开发前一定要**先写开发文档**。特别是多人合作的项目。
* 有什么新的进展在这里更新。

## 项目结构

采用Gulp前端工程化，主要实现自动编译Sass，压缩JS和CSS。

    PicSite
    │
    ├─dist # 工程化后导出的文件目录
    │  ├─css # 压缩后的CSS文件
    │  └─js # 压缩后的JS文件
    │
    ├─node_modules # 开发时通过npm安装的各种包
    │
    ├─src # 源文件
    │   ├─css # 将Sass编译后的CSS文件
    │   ├─js # JS文件
    │   └─sass # 未编译的Sass文件
    │ 
    ├─.gitignore # git忽略文件
    ├─ design.md # 设计图（包含很图片）
    ├─ gulpfile.js # gulp文件，实现自动化编译和压缩静态文件
    ├─ index.html # 首页
    ├─ LICENSE # 许可证
    ├─ package.json # 依赖包信息
    └─ README.md # 说明及开发文档

