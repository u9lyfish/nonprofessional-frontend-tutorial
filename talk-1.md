
## Warm up

### Task 1

从当前 URL 地址取得 get 请求参数，并包装成对象形式。

例子：

- 当前 URL 地址为：`http://example.com/index.htm?name=lyy&age=26`
- 输出：`{ name: 'lyy', age: '26' }`

### Task 2

实现 Pinterest 瀑布流，考虑实现中的注意点，提出性能优化方法

## 前端是什么

范畴：所有发生在浏览器内的事

### 典型的前端开发工作：

1. Web API
2. 字符串、数组、对象的处理
3. 函数式编程风格
4. Ajax 请求
5. DOM 操作，CSS 样式
6. 表单交互与验证

### 今天前端能做什么

- Web 网页开发
    - 地理位置, 加速度, 蓝牙, NFC, ...
    - WebSocket, LocalStorage, WebGL, ...
    - [https://whatwebcando.today/](https://whatwebcando.today/)
- Hybrid App 开发
- Native App 开发：ReactNative / Weex
- Node.js 后端开发

## 发展历史

前端发展的历史 = 填坑的历史

几大天坑：

1. JavaScript 语言本身不支持模块化
2. HTML/CSS/JavaScript 标准不支持组件化
3. DOM 的渲染、重绘过程效率差
4. 浏览器市场横向分裂（IE/C/FF/S/O）、纵向分裂（历史兼容问题）

### 石器时代

- 手动处理浏览器兼容性
- 手动管理依赖和加载顺序

### 启蒙时代

jQuery：

- 抹平浏览器兼容性差异
- 封装 Web API
- 链式调用语法

初步实现模块化：

- 自动管理依赖
- 实现异步加载

### 文艺复兴

Google 复兴 Ajax 技术：

- 不必等全部内容加载完即可显示 - 更快
- 不必刷新即可更新内容 - 更流畅
- 不必由后端渲染页面 - 更轻量

为什么要前后端分离：

- 页面变成静态资源，提高加载速度
    - 利于缓存
    - 减少后端计算量
- 数据使用 Ajax 更新，不阻塞 UI，改善体验
- 开发耦合度低

### 工业革命

AngularJS：

- 复兴 MVVM 模型
- √ 业务逻辑与 UI 分离
- √ 利于测试
- x 性能问题
- x 组件化不够彻底

其他框架参见 [ToDoMVC](http://todomvc.com/)

### 人类英雄

React：

 - MVC 模型中的 V (View)
 - 数据单向流动
 - √ Virtual-DOM-diff 算法提升性能
 - √ JSX + WebPack 实现彻底组件化

JSX -> Virtual DOM -> Real DOM / Native iOS / Native Android

ReactNative:

 - Native, not hybrid
 - 用 native JavaScript 引擎解释执行
 - JavaScript <-> JSBridge <-> Native Code
 - ...

## 工欲善其事

前端开发常用工具

### 命令行工具

 - npm: 依赖管理工具
 - WebPack: 构建、打包工具
 - Babel: 转译工具

### IDE / 文本编辑器

 - WebStorm
 - Sublime / Atom
 - ...

### 调试工具：浏览器

 - Chrome DevTools
