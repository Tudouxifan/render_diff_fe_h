- 服务启动文件：app.ts , 修改服务启动的端口号 也在这里配置

- 启动方式
    * `npm run client:dev` dev 打包 📦 前端代码 （开发环境用）
    * `npm run client:prod` prod 打包 📦 前端代码（生产环境用）
    * `npm run dev` 前台启动 node 应用
- 项目文件介绍
    - 前端依赖包目录：node_modules, 我们开发过程中不会管他，是执行 npm install 自动生成的
    - 依赖包有那些在 package.json 里面有定义，可以单独安装一些依赖：npm install xxx --save-dev / npm install xxx --save, 安装好后会自动写入package.json 
    - config 目录：前端打包的配置文件目录
    - constant 目录: 配置常量的目录
    - controller 目录： 控制器（接口转发） 前端请求-》node（controller）-》python（or 其他后端接口）
    - dist 目录：是前端打包的产物（把 src里面的东西给打包到dist）
    - interface、ioc、service 目录：抽象接口，属于项目底层架构设计
    - util 目录：工具目录

    - src/webapp 目录： 前端代码源文件目录，我们写的页面全部在这里面
    - **配置前端路由的地方：src/webapp/containers/index.js**
    - 组件目录：src/webapp/components
    - 前端静态目录（放一些图片类的资源）:src/webapp/static
    - 状态管理：src/webapp/store