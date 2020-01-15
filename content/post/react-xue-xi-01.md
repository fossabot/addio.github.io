---
title: 'React 学习 day 1'
date: 2020-01-14 14:15:56
tags: [前端,react,学习]
published: true
hideInList: false
feature: /post-images/react-xue-xi.png
isTop: false
---

React 是一个用于构建用户界面的 JavaScript 库。这是一个学习React的笔记

<!-- more -->

# 环境：Node.js

```
node -v
npm -v
```
# 创建项目：[Create React App][1]

```
npx create-react-app my-app
cd my-app
npm start
```

![屏幕截图(2).png](https://raw.githubusercontent.com/addio/addio.github.io/assets/images/%E5%B1%8F%E5%B9%95%E6%88%AA%E5%9B%BE(2).png)

## 项目初始化目录介绍

### 入口文件  my-app/src/index.js

```
import React from 'react';
import ReactDOM from 'react-dom';
import './index.css';
import App from './App';
import * as serviceWorker from './serviceWorker';

ReactDOM.render(<App />, document.getElementById('root'));

// If you want your app to work offline and load faster, you can change
// unregister() to register() below. Note this comes with some pitfalls.
// Learn more about service workers: https://bit.ly/CRA-PWA
serviceWorker.unregister();
```

# 写个Hello World!

1. 清空src内文件

2. 创建src/index.js

```
import React from "react";
import ReactDOM from "react-dom";
import App from './App';

ReactDOM.render(<App />, document.getElementById("root"));
```

3. 创建src/App.js

```
import React, { Component } from "react";

class App extends Component {
  render() {
    return <div>Hello World!</div>;
  }
}
```

[1]: https://zh-hans.reactjs.org/docs/create-a-new-react-app.html "React"
