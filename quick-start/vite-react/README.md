# 使用官方脚手架创建一个 Vite + React 项目

## 1. 步骤

1. 执行脚手架命令：

```shell
$ npm create vite@latest

✔ Project name: … vite-react
✔ Select a framework: › React
✔ Select a variant: › TypeScript

Scaffolding project in /xxx/vite-react...

Done. Now run:

  cd vite-react
  npm install
  npm run dev
```

2. 安装依赖

```shell
$ cd vite-react
$ npm install
```

3. 启动开发

```shell
$ npm run dev

> vite-react@0.0.0 dev
> vite

  VITE v4.4.9  ready in 218 ms

  ➜  Local:   http://localhost:5173/
  ➜  Network: use --host to expose
  ➜  press h to show help
```

4. 执行构建

```shell
$ npm run build

> vite-react@0.0.0 build
> tsc && vite build

vite v4.4.9 building for production...
✓ 34 modules transformed.
dist/index.html                   0.46 kB │ gzip:  0.30 kB
dist/assets/react-35ef61ed.svg    4.13 kB │ gzip:  2.14 kB
dist/assets/index-d526a0c5.css    1.42 kB │ gzip:  0.74 kB
dist/assets/index-c7e05d32.js   143.41 kB │ gzip: 46.10 kB
✓ built in 454ms
```

## 2. 理解

1. 以 `index.html` 作为入口文件，Vite 解析其 `<script type="module" src="...">` 标签指向源码 `./src/main.tsx`。
2. 在 `./src/main.tsx` 中引入各类资源，渲染 React 组件并挂载在 `#root` 元素之上。
3. 在 `./vite.config.ts` 中配置 React 插件以让 Vite 支持 React 语法。
