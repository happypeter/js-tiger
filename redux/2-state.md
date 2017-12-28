# 使用内部 state 实现商品列表


### 添加 Products 组件

分为展示和容器两部分来写。

products---

Main.js 中导入容器组件 ProductsContainer ，放到下面显示。

添加 containers/ProductsContainer.js 文件。里面写成一个简单的函数式组件，显示出展示组件 Products 。

添加展示组件 components/Products.js 文件。里面写一个 class 组件
，显示一个占位符字符串 Products 。

浏览器中，显示出了 Products 字符串。

### 使用组件内 state 做数据

来显示一个商品列表。

product-list---

到 components/Products.js 中， state 中添加一个常量 products ，是一个对象数组，每一个 product 对象，包含 id 和 name 两项内容。下面，解构赋值拿到 products ，map 一下，把生成的 jsx 赋值到 productList 常量，并最终在 return 语句中显示出来。

浏览器中，看到商品列表显示出来了。
