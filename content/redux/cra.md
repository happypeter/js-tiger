# 搭建 create-react-app 环境

先来搭建 creact-react-app 的基本环境。

保证系统上安装了 creact-react-app 之后，运行：

```
create-react-app redux-cart
```


fresh-cra---

运行 npm start 启动一下。

到浏览器中，localhost:3000 端口，可以看到一个带 react 图标的启动画面。


### 区分展示组件和容器组件

按照[展示组件和容器组件](http://haoduoshipin.com/videos/236) 的思路，把项目结构调整一下。


refactor---


删除整个的 src 文件夹，重新创建 src/index.js 。里面导入 ReactDOM 显示出 App 组件。

 App.js 作为容器组件，放到 src/containers 文件夹中，删除里面的 jsx 内容，只显示 Main 组件。

Main.js 定义在 src/components/ 中，里面暂时先显示一个 Hello 。

浏览器中，看到 Hello 依然能够显示，表示重构成功。
