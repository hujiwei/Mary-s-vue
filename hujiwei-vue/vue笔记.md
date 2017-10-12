# vue命令行安装

```shell
# npm版本3.*，高版本的npm安装vue时会有奇怪的错误 (⊙﹏⊙)b
$ npm install vue -g
$ npm install vue-cli -g
```

# 创建项目

```shell
# 创建一个基于 webpack 模板的新项目
$ vue init webpack my-project
# 安装依赖，走你
$ cd my-project
$ npm install
$ npm run dev
```

# 安装element-ui

element-ui是饿了么团队开发的一个基于vuejs的ui组件库，pc端的，相当好用

```shell
# 安装 
npm i element-ui -S
```

完整引入，在main.js中写入下面内容

```js
import Vue from 'vue'
import ElementUI from 'element-ui'
import 'element-ui/lib/theme-default/index.css'
import App from './App.vue'

Vue.use(ElementUI)

new Vue({
  el: '#app',
  render: h => h(App)
})
```

关于element-ui完整文档，请查看[官方文档](http://element.eleme.io/#/zh-CN/component/installation)

# 安装less

```shell
# 安装less
npm install less less-loader -D
```

# 安装sass

```shell
# 安装sass
npm install sass-loader -D
# sass-loader依赖于node-sass
npm install node-sass -D
```
