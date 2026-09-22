# React Bits Fork 维护工作流

这个 Fork 用于维护个人的 React Bits 组件来源和前端实验流程。

## 分支职责

- `main`：只跟踪 `DavidHDev/react-bits` 上游。
- `codex-custom`：保存中文说明、Codex 使用边界和个人维护文档。
- `feature/*`：一次具体的组件修改或实验。

不要把完整的 React Bits 仓库复制进业务项目；业务项目只添加实际使用的组件。

## 同步上游

在 GitHub 网页中打开本 Fork，使用文件列表上方的 **Sync fork**。

命令行同步：

```bash
git clone https://github.com/funny910/react-bits.git
cd react-bits
git remote add upstream https://github.com/DavidHDev/react-bits.git
git fetch upstream
git switch main
git merge --ff-only upstream/main
git push origin main
```

如果 `main` 有本地修改，先把修改移到 `codex-custom` 或 feature 分支，再同步上游。

## 组件改动原则

1. 先确认组件是否已经存在，避免重复实现。
2. 组件源代码、示例和构建输出分开处理。
3. 不在上游同步分支里混入个人视觉实验。
4. 每个组件改动保留一个最小构建或页面检查。
5. 需要贡献回上游时，先遵守原仓库的贡献要求。
