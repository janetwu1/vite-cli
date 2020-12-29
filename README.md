# vite-cli
Vite实现原理
#### vite概念

- vite是一个面向现代浏览器的一个更轻、更快的Web应用开发工具
- 它基于ECMAScript标准原生模块系统（ES Modules）实现

#### vite项目依赖

- vite
- @vue/compiler-sfc

#### 基础使用

- vite serve

  - 是一个用于启动web开发的服务器，启动服务器的时候不需要编译所有的代码文件，启动非常快



- Vite build

  - Rollup
  - Dynamic import
    - Polyfill



#### vite核心功能

- 静态Web服务器
- 编译单文件组件
  - 拦截浏览器不识别的模块，并处理
- HMR
  - vite HMR
    - 立即编译当前所修改的文件
  - Webpack HMR
    - 会自动以这个文件为入口重写build一次，所有的涉及到的依赖也都会被加载一遍


#### vite特性

- 快速冷启动
- 模块热更新
- 按需编译
- 开箱即用
  - TypeScript-内置支持
  - less/sass/stylus/postcss-内置支持（需要单独安装）
  - jsx
  - Web Assembly



