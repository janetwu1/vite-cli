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

    

  ![image-20201228174540116](images/image-20201228174501500.png)

  ![image-20201228174621623](images/image-20201228174621623.png)

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



##### 打包Or不打包

- 使用Webpack打包的两个原因
- 浏览器环境并不支持模块化
- 零散的模块文件会产生大量的HTTP请求

##### 浏览器对ES Module的支持

![image-20201228175730919](images/image-20201228175730919.png)





#### vite特性

- 快速冷启动
- 模块热更新
- 按需编译
- 开箱即用
  - TypeScript-内置支持
  - less/sass/stylus/postcss-内置支持（需要单独安装）
  - jsx
  - Web Assembly

```
npm i @vue/compiler-sfc
```





```
shared:387 Uncaught ReferenceError: process is not defined
    at shared:387
```

