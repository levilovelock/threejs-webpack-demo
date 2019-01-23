# three.js + webpack4 demo

- 测试以es6语法，使用webpack4打包three.js应用

## 运行应用

```bash
# 安装package.json的依赖包
$ npm install

# 运行应用
$ npm run start

# 打包应用
$ npm run build

# 完成打包后打包的应用位于dist/目录，可以直接运行查看效果
$ ls -l dist
total 992
-rw-r--r--  1 cookeem  staff  500492  1 23 15:52 bundle.js
-rw-r--r--@ 1 cookeem  staff     183  1 23 15:52 index.html
```

## 如何创建package.json

```bash
# 初始化npm包
$ npm init

# 安装包webpack依赖包
$ npm install webpack webpack-cli webpack-dev-server html-webpack-plugin -D --save

# 安装es6支持
$ npm install babel-loader@8 @babel/core @babel/preset-env -D --save

# 安装three.js
$ npm install three.js -D --save

# 设置package.json
$ vi package.json
  "scripts": {
    "start": "webpack-dev-server --mode development --open",
    "build": "webpack --mode production"
  },
```
