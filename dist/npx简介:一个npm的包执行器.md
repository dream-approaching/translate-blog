# npx 简介:一个 npm 的包执行器

原文：[Introducing npx: an npm package runner](https://medium.com/@maybekatz/introducing-npx-an-npm-package-runner-55f7d4bd282b)  
作者：[Kat Marchán](https://medium.com/@maybekatz)  
时间：2017 年 7 月 11 日

---

那些将 npm 升级到最新版本[`npm@5.2.0`](https://github.com/npm/npm/releases/tag/v5.2.0)的人可能会注意到，这次版本除了通常的`npm`之外还安装了一个新的二进制文件：[`npx`](https://www.npmjs.com/package/npx)

npx 是一个工具，它旨在提高从 npm 注册表中使用软件包的体验，就和 npm 使得安装和管理贮存在注册表中的依赖变得十分简单一样，npx 使得使用 CLI 工具和其他贮存在注册表中的可执行文件变得容易。它极大地简化了许多操作，这些操作就算现在单单用 npm 的话也要执行一些必要的“仪式”。

### 使用本地安装的工具，不执行 npm run-script

![](https://github.com/dream-approaching/translate-blog/blob/master/assets/gif1.gif)
将 cowsay 作为本地 devDependency 进行安装，并使用 npx cowsay 来运行它
