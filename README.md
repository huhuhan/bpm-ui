## bpm-ui静态前端

### 简介

- 本项目作为静态前端，主要用其中的flow-editor流程设计器和表单模块，正常情况不用构建编辑

  

### 安装
 ```shell
  npm install
 ```
> 不用在意python之类的报错。但build目录下的font、images不能删去
> 解决问题后，.gitignore里将build目录过滤掉

### 构建
 ```shell
  npm run build
 ```
- assets/app-conf.js 中配置后端服务，代理转发前缀
- 根据webpack.config的配置得知，assets目录下就是构建后的文件

  
### 区别

基于开源版本1.23
- 修改了部分页面的请求方式，参考git历史
- 修改了代理转发配置
- 。。。。

## 开源项目

### 简介
- AgileBPM中的[前端模块](https://gitee.com/agile-bpm/agile-bpm-basic/tree/master/bpm-explorer)

- 前端项目非单页面应用，而且系统为了入手更容易，仅仅对公共js 模块化打包，并暴露关键框架的全局引用。
   当在开发的时候，不需要关注公共模块的js，你可以直接引入自己的js。

- 开发参考
  
  - 列表页面可参考 sysPropertiesList.html
  - 编辑页可参考 sysPropertiesEdit.html

- 运行
  - 前后端一起开发的推荐 通过Tomcat 运行前端资源
  - 前端独立开发的，推荐 	`npm run dev ` 运行前端项目
