# vue-admin-template（后台项目基于此开发）

> 这是一个极简的 vue admin 管理后台。它只包含了 Element UI & axios & iconfont & permission control & lint，这些搭建后台必要的东西。

[线上地址](http://zybank-fe.github.io/vue-admin-template)

## Extra

如果你想要根据用户角色来动态生成侧边栏和 router，你可以使用该分支[permission-control](https://github.com/zybank-fe/vue-admin-template/tree/permission-control)

## 相关项目

[vue-element-admin](https://github.com/zybank-fe/vue-element-admin)

[electron-vue-admin](https://github.com/zybank-fe/electron-vue-admin)

[vue-typescript-admin-template](https://github.com/zybank-fe/vue-typescript-admin-template)

## Build Setup

```bash
# 克隆项目
git clone https://github.com/zybank-fe/vue-admin-template.git

# 进入项目目录
cd vue-admin-template

# 安装依赖
npm install -g yarn

# 建议不要直接使用 cnpm 安装以来，会有各种诡异的 bug.
yarn install --registry=https://registry.npm.taobao.org

# 启动服务
yarn run dev
```

浏览器访问 [http://localhost:9528](http://localhost:9528)

## 发布

```bash
# 构建测试环境
yarn run build:stage

# 构建生产环境
yarn run build:prod
```

## 其它

```bash
# 预览发布环境效果
yarn run preview

# 预览发布环境效果 + 静态资源分析
yarn run preview -- --report

# 代码格式检查
yarn run lint

# 代码格式检查并自动修复
npm run lint -- --fix
```

更多信息请参考 [使用文档](https://panjiachen.github.io/vue-element-admin-site/zh/)

## Demo

![demo](https://github.com/PanJiaChen/PanJiaChen.github.io/blob/master/images/demo.gif)

## Browsers support

Modern browsers and Internet Explorer 10+.

| [<img src="https://raw.githubusercontent.com/alrra/browser-logos/master/src/edge/edge_48x48.png" alt="IE / Edge" width="24px" height="24px" />](http://godban.github.io/browsers-support-badges/)</br>IE / Edge | [<img src="https://raw.githubusercontent.com/alrra/browser-logos/master/src/firefox/firefox_48x48.png" alt="Firefox" width="24px" height="24px" />](http://godban.github.io/browsers-support-badges/)</br>Firefox | [<img src="https://raw.githubusercontent.com/alrra/browser-logos/master/src/chrome/chrome_48x48.png" alt="Chrome" width="24px" height="24px" />](http://godban.github.io/browsers-support-badges/)</br>Chrome | [<img src="https://raw.githubusercontent.com/alrra/browser-logos/master/src/safari/safari_48x48.png" alt="Safari" width="24px" height="24px" />](http://godban.github.io/browsers-support-badges/)</br>Safari |
| --------- | --------- | --------- | --------- |
| IE10, IE11, Edge| last 2 versions| last 2 versions| last 2 versions

## License

[MIT](https://github.com/PanJiaChen/vue-admin-template/blob/master/LICENSE) license.

Copyright (c) 2017-present PanJiaChen
