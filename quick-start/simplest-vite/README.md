# 使用官方脚手架创建一个最简单的 Vite 项目

备注： 单词 “Vanilla”，在编程语言中通常指的是没有任何框架或者库的纯粹、原始的编程语言。这个词汇源于冰淇淋的香草味，意指基础、原始、未经修改的版本。Vite 脚手架在选择模板时，选项 “Vanilla” 就是指没有使用任何 JavaScript 库或框架的纯 JavaScript 模板。

1. 执行脚手架命令：

```shell
$ npm create vite@latest

Need to install the following packages:
  create-vite@4.4.1
Ok to proceed? (y) y

✔ Project name: … simplest-vite
✔ Select a framework: › Vanilla
✔ Select a variant: › TypeScript

Scaffolding project in /.../simplest-vite...

Done. Now run:

  cd simplest-vite
  npm install
  npm run dev
```

2. 安装依赖

```shell
$ cd simplest-vite
$ npm install
```

3. 启动开发

```shell
$ npm run dev

> simplest-vite@0.0.0 dev
> vite

  VITE v4.4.9  ready in 109 ms

  ➜  Local:   http://localhost:5173/
  ➜  Network: use --host to expose
  ➜  press h to show help
```
