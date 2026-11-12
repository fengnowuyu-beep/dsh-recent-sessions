# dsh-recent-sessions

一个 DSH 插件：在侧边栏「工作区」列表顶部插入「最近」分组，把分散在各个工作区里的最近会话收拢到一处。

本仓库是从 [kyrsieger/dsh-up-session](https://github.com/kyrsieger/dsh-up-session) 定制的分支，只保留「最近」，已移除「置顶」。

## 文档参考

- [术语表](./GLOSSARY.md)：项目领域术语的定义，以及同一概念的用词取舍。
- [文档目录](./docs/)：功能设计及其他项目文档。
- [ADR 目录](./docs/adr/)：架构决策记录，说明难以逆转的设计决定及其背景。

## README 多语言

中文 [README.md](./README.md) 是默认版本，英文版本为 [README.en.md](./README.en.md)。修改 README 时必须同步修改其他语言版本，保持各版本内容一致（语言切换行、截图等结构也需对齐）。

## 兼容版本

修改 `package.json` 中的 `engines.dsh` 兼容版本时，必须同步修改中文 README「安装与兼容」和英文 README「Installation and compatibility」章节第一行的版本号，保持一致。

## CHANGELOG

上游条目里的 PR 与 issue 链接指向 `kyrsieger/dsh-up-session`；本分支自己的改动不虚构上游链接。生成 CHANGELOG 时如某项来自本仓库的 PR/issue，附上对应链接。
