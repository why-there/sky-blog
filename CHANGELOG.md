# 版本日志

## 2026-06-04

### 仓库初始化

- 站点标题：`月亮加盐` → `天空有痕迹`
- 仓库引用：所有 `moon-blog` 引用统一替换为 `sky-blog`（hugo.yaml、go.mod、pages.yaml、README.md、content/_index.md）
- 删除 `AGENTS.md`
- 移除 `hugo.yaml` 文件开头的 UTF-8 BOM（修复 CI 构建失败）

### 功能变更

- 点击导航栏头像跳转到「关于」页面（logo.link: `/` → `/about`）
