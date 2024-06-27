# 现代化的 Chrome 扩展程序 Vite Starter

> 由 [Vite](https://vitejs.dev/) 驱动的 `现代化 Chrome 扩展程序 Manifest V3` ([Chrome](https://developer.chrome.com/docs/extensions/mv3/getstarted/))  入门模板。

|  页面类型   |                                                             浅色模式                                                              |                                                             深色模式                                                              |
| :----------: | :---------------------------------------------------------------------------------------------------------------------------------: | :--------------------------------------------------------------------------------------------------------------------------------: |
|  弹出页面  |  ![](https://cdn.jsdelivr.net/gh/xiaoluoboding/image-hub-for-repo@latest/chrome-ext-mv3-starter/202107_extpreview_popup_light.png)  |  ![](https://cdn.jsdelivr.net/gh/xiaoluoboding/image-hub-for-repo@latest/chrome-ext-mv3-starter/202107_extpreview_popup_dark.png)  |
| 选项页面 | ![](https://cdn.jsdelivr.net/gh/xiaoluoboding/image-hub-for-repo@latest/chrome-ext-mv3-starter/202107_extpreview_options_light.png) | ![](https://cdn.jsdelivr.net/gh/xiaoluoboding/image-hub-for-repo@latest/chrome-ext-mv3-starter/202107_extpreview_options_dark.png) |

## 特性

- ⚡️ **即时 HMR** - 在开发时使用 **Vite** (不再需要刷新！)
- 🥝 Vue 3 - Composition API，[`<script setup>` 语法](https://github.com/vuejs/rfcs/blob/master/active-rfcs/0040-script-setup.md) 等等！
- 💬 轻松通信 - 由 [`webext-bridge`](https://github.com/antfu/webext-bridge) 和 [VueUse](https://github.com/antfu/vueuse) 存储提供支持
- 🍃 [Windi CSS](https://windicss.org/) - 按需 CSS 工具
- 🦾 [TypeScript](https://www.typescriptlang.org/) - 类型安全
- 📦 [组件自动导入](./src/components)
- 🌟 [图标](./src/components) - 直接访问来自任何图标集的图标
- 🌍 [I18N 就绪](src/locales)
- 🌛 深色模式 - 支持切换深色模式
- 📃 具有完整类型支持的动态 `manifest.json`

## 预先打包

### WebExtension 库

- [`webextension-polyfill-ts`](https://github.com/Lusito/webextension-polyfill-ts) - 具有类型的 WebExtension 浏览器 API Polyfill
- [`webext-bridge`](https://github.com/antfu/webext-bridge) - 上下文之间的轻松通信

### Vite 插件

- [`vite-plugin-components`](https://github.com/antfu/vite-plugin-components) - 组件自动导入
- [`vite-plugin-windicss`](https://github.com/antfu/vite-plugin-windicss) - WindiCSS 支持
- [`@intlify/vite-plugin-vue-i18n`](https://github.com/intlify/bundle-tools/blob/main/packages/vite-plugin-vue-i18n/README.md) - i18n 支持

### Vue 插件

- [`vue-global-api`](https://github.com/antfu/vue-global-api) - 全局使用 Vue Composition API
- [VueUse](https://github.com/antfu/vueuse) - 有用的组合 API 集合

### UI 框架

- [Windi CSS](https://github.com/windicss/windicss) - 下一代实用优先的 CSS 框架

### 图标

- [Iconify](https://iconify.design) - 使用来自任何图标集的图标 [🔍Icônes](https://icones.netlify.app/)
- [`vite-plugin-icons`](https://github.com/antfu/vite-plugin-icons) - 将图标作为 Vue 组件

### 编码风格

- 将 Composition API 与 [`<script setup>` SFC 语法](https://github.com/vuejs/rfcs/pull/227) 一起使用
- [ESLint](https://eslint.org/) 与 [@antfu/eslint-config](https://github.com/antfu/eslint-config)，单引号，无分号

### 开发工具

- [TypeScript](https://www.typescriptlang.org/)
- [pnpm](https://pnpm.js.org/) - 快速、节省磁盘空间的包管理器
- [tsup](https://github.com/egoist/tsup) - 由 esbuild 提供支持的零配置 TypeScript 打包器
- [esno](https://github.com/antfu/esno) - 由 esbuild 提供支持的 TypeScript / ESNext 节点运行时
- [npm-run-all](https://github.com/mysticatea/npm-run-all) - 并行或顺序运行多个 npm 脚本

## 使用模板

### GitHub 模板

[从 GitHub 上的此模板创建仓库](https://github.com/xiaoluoboding/chrome-ext-mv3-starter/generate).

### 克隆到本地

如果您更喜欢使用更简洁的 git 历史手动执行此操作

> 如果您没有安装 pnpm，请运行：npm install -g pnpm

```bash
npx degit xiaoluoboding/chrome-ext-mv3-starter my-extension
cd my-extension
pnpm i
```

## 用法

### 文件夹

- `src` - 后台脚本和内容脚本以及扩展程序的前端（弹出窗口和选项）。
  - `manifest.ts` - 扩展程序的清单。
- `extension` - 扩展程序包根目录，也存放资产。
- `scripts` - 开发辅助脚本。

### 开发

```bash
pnpm dev
```

然后 **使用 `extension/` 文件夹在浏览器中加载扩展程序**,

### 构建

要构建扩展程序，请运行

```bash
pnpm build
```

然后将文件打包到 `extension` 下。

## 致谢

这是一个源自 [antfu/vitesse-webext](https://github.com/antfu/vitesse-webext) 的模板

## 谁在使用这个模板？

- [chrome-web-bookmark](https://github.com/xiaoluoboding/chrome-web-bookmark) -  Chrome 扩展程序可以将链接转换为可视化书签。

## 许可证

[MIT](./LICENSE) - [@xiaoluoboding](https://github.com/xiaoluoboding)