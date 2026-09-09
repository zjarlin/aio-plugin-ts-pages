# TypeScript Static Pages

这是 TypeScript `page-definition` 插件。类型化模型生成 `dist/pages.json`，宿主在安装时校验并挂载页面，不创建运行实例。

```bash
corepack enable
pnpm install --frozen-lockfile --ignore-scripts
pnpm typecheck
pnpm test
pnpm build
aio plugin validate
```

发布前提交 `pnpm-lock.yaml` 和 `dist/pages.json`；静态页面插件不能声明动作页面。
