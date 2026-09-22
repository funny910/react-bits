# 在 Codex 中使用 React Bits

React Bits 是组件库，不是一个需要每次对话调用的 Codex skill。使用时，在具体 React 项目中明确组件名称和项目路径：

```text
在 <project-root>/react-bits-demo 中，
添加 React Bits 的 BlurText TypeScript 版本，并接入当前页面。
```

官方支持通过 shadcn、jsrepo 或手动复制组件：

```bash
npx shadcn@latest add @react-bits/BlurText-TS-TW
```

## 推荐边界

- React Bits Fork：保存上游源码和个人组件研究。
- 业务项目：只保存实际使用的组件和它们需要的依赖。
- Demo 项目：独立展示组件效果，不反向污染 Fork 的 `main`。
- Codex 的 UI/UX 设计工作：使用 `$ui-ux-pro-max` 或 `$impeccable`，不要把组件库当成设计审查 skill。

添加组件后至少运行：

```bash
npm run build
```
