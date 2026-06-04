# 版本日志

## 2026-06-04

### 仓库初始化

- 站点标题：`月亮加盐` → `天空有痕迹`
- 仓库引用：所有 `moon-blog` 引用统一替换为 `sky-blog`（hugo.yaml、go.mod、pages.yaml、README.md、content/_index.md）
- 删除 `AGENTS.md`
- 移除 `hugo.yaml` 文件开头的 UTF-8 BOM（修复 CI 构建失败）

### 功能变更

- 点击导航栏头像跳转到「关于」页面（logo.link: `/` → `/sky-blog/about/`）
- 浏览器页签图标（favicon）改为使用头像图片：新增 `layouts/_partials/favicons.html` 覆盖主题默认模板

### 修复

- 头像圆形显示失效：修改 `custom.css` 选择器，去掉 `a[href="/"]` 精确匹配，改为直接匹配 `img[src*="Avatar"]`
