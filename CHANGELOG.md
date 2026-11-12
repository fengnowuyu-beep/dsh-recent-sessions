# 更新日志

## 0.1.0 - 2026-11-12

本版本从上游 `kyrsieger/dsh-up-session` 1.2.2 分叉并更名为 `dsh-recent-sessions`，只保留「最近」功能。

### 变更

- 移除置顶区（`PinnedSection`）、置顶/取消置顶行操作与「显示置顶」设置；最近区不再排除已置顶会话。
- 移除置顶相关的图标、样式、词典条目与测试断言。
- 命名空间、CSS 前缀、本地存储键、插槽 key、模块 id 全部改为 `dsh-recent-sessions` / `dshRS-`。
- 兼容版本声明调整为 `engines.dsh: ">=0.2.2-rc.2"`。

### 修复

- 继承上游 1.2.2 的 rc.2 侧栏修复：以宿主显式标记的 `[data-sidebar-list-area]` 作为滚动落点，不再依赖会随内容与滚动状态变化的 `overflow-y`，避免「插入—移除」反复挂载导致分组闪动或消失。
- 测试脚本改为容忍 CRLF（Windows 检出时 `inject,\n apply,` 的注入锚点原本匹配不到，测试会在本机误报失败）。
