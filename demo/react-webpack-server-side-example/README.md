# react-webpack-server-side-example

react && webpack && server-side app

## 开发环境


1. 需要 `node && npm` 。可以通过同级目录下的`node`进行一键安装
2. 将代码复制到自己的开发目录下
3. `npm install`安装项目需要的依赖
4. `npm start`启动项目
5. `npm run production`编译生产环境代码

## 预览

webpack 编译需要两个独立的配置：一个是浏览器打包的配置，另外一个是服务器渲染的配置。服务端的包可以在其它`node.js`代码来引用构建预呈现的HTML。
## 特色

* Same react code (`app/Application.js`) run on server and on client
* 在这两种情况下，代码都是通过`Webpack`来编译的
  * 支持加载器，如：资源的文件加载器 
* 服务端的编译收集样式并把他们包含在预渲染的`HTML`代码中。
  * This avoids FOUC of the pre-rendered HTML
* 浏览器构建包含了一个用于缓存的 hash 浏览器地址。
## 使用

``` 
npm install
``` 
安装依赖

`npm start`

执行的是 `webpack --progress && node server`


1. 编译浏览器软件包和服务端软件包。它还将浏览器包的统计信息存储为json文件。
2. 运行服务。服务需要服务端的包来为每个请求生成HTML。它还读取浏览器包的文件名以插入`<script>`标签。

### 产品

``` 
npm run production
```

这个命令是用来编译生产版本的浏览器包和服务端包。并且会压缩`Javascript`和`css`代码。
