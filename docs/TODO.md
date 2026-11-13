# TODO

> 待办登记：日期 / 内容 / 目标文件 / 完成状态。按协作规则「TODO 必须 md 记录」建立。

| 日期 | 内容 | 目标文件 | 完成状态 |
| --- | --- | --- | --- |
| 2026-11-13 | 本机安装 Docker Desktop 并启用 WSL2 后端（当前无 Docker、WSL 无发行版），验证 `docker compose version` | 本机环境（无仓库文件） | 未开始，需用户在本机执行 |
| 2026-11-13 | 修复 corepack 0.31.0 与 pnpm 12.3.4 不兼容：切到 Node 22.22.2 后 `corepack install`，验证 `corepack pnpm -v` = 12.3.4 | 本机环境（无仓库文件） | 未开始，需用户在本机执行 |
| 2026-11-13 | 执行 `corepack pnpm install --frozen-lockfile`，并准备根目录 `.env` | 本机环境 / `.env` | 未开始，依赖前两项 |
| 2026-11-13 | 阶段 1 验收：`corepack pnpm --filter @ai-se/mcp typecheck && lint && test`、`--filter @ai-se/database migrate`、`/health`、`/ready`、Web 列表页 | `packages/mcp`、`packages/database`、apps | 未开始，依赖前三项 |
| 2026-11-13 | Windows 适配下一阶段：`build:image` 使用 POSIX 参数展开 `${PREWARM_PACKAGES:+...}`，Windows 下不可用 | `packages/sandbox/package.json` | 未开始（STOP，未获授权） |
| 2026-11-13 | Windows 适配下一阶段：`DockerSandbox` 把宿主路径拼成 `${workspace}:/workspace`，Windows 盘符需 Docker Desktop 风格转换，否则 Agent/Sandbox 执行链不可用 | `packages/sandbox/src/index.ts` | 未开始（STOP，未获授权） |
| 2026-11-13 | 待确认：是否需要 `dev:win` 一键入口（新增 `infrastructure/windows/dev.ps1` + 根脚本），还是保持手册里的 PowerShell 分步 | 根 `package.json`、`infrastructure/` | 待确认，不阻塞其余 |
