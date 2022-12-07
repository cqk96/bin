# ad_admin

## Project setup
```
npm install
```
第一次拉取代码时执行,前提是安装了node,node自行安装百度一大堆,node版本是v14.5.0
npm版本是跟随你node改变
nvm node版本管理工具(不是强制下,提一嘴,方便切换node版本,基本上专业前端用的多)
### Compiles and hot-reloads for development
```
npm run serve
```
环境安装好之后执行,代码热更新,不需要刷新页面.除非你代码除了问题
### Compiles and minifies for production
```
npm run build
```
打包命令,业务代码写完之后执行打包命令
### Lints and fixes files
```
npm run lint
```
这是暂时没用到,想了解自行百度
### Customize configuration
See [Configuration Reference](https://cli.vuejs.org/config/).


### 自定义添加请求
``` 
this.$http
```
简单封装了一下请求,拿来可以直接使用
this.$http('GET','/xx/xx',{param1:'',param2:''}).then(res=>{console.log(res)})


### 自定义添加配置
```
.env config.js  
```
直接把备份拿出来即可,.env文件中的DEV_URL配置自己本地的测试域名（要加上协议头http://）,跨域也搞过了,不出问题的话可以直接使用