# agileBPM前端项目
## 原项目说明 
前端项目非单页面应用，而且系统为了入手更容易，仅仅对公共js 模块化打包，并暴露关键框架的全局引用。
当在开发的时候，不需要关注公共模块的js，你可以直接引入自己的js。
### 定义开发
- 列表页面可参考 sysPropertiesList.html
- 编辑页可参考 sysPropertiesEdit.html

## 安装
` npm install`

> 不用在意python之类的报错。
## 构建
- assets/app-conf.js 中配置后端服务 前缀、默认为 /  
- 跨域需要修改为具体后端请求地址: http://.....
- flow-editor/editor-app/app-cfg.js  中配置流程设计器的后端服务前缀、默认为 /
- **测试地址：http://192.168.0.82:8555**
- 修改公共 js 后需要手动打包   `npm run build`

## 运行
允许前端项目有两种形式
- 前后端一起开发的推荐 通过Tomcat 运行前端资源
- 前端独立开发的，推荐 	`npm run dev ` 运行前端项目

