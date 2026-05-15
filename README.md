# BiliNote-CLI.skill
让 AI Agent 自动调用 [BiliNote-CLI](https://github.com/FisherRone/BiliNote-CLI) 为你的视频生成结构化 Markdown 笔记。

> 只需要把视频链接丢给 Agent，它就会完成转写、总结、生成笔记 — 你什么都不用管。

## ✨ 能做什么

- 把 B 站、YouTube、抖音、快手甚至本地视频变成笔记
- 在 B 站搜索某个主题，批量生成调研报告
- 自动插入截图、跳转链接，可选多模态理解画面
- 支持学术风、口语风等多种笔记风格

## ⚙️ 前置条件

这个 skill 本身只是一段指导 AI 的提示词，真正干活的是 [BiliNote-CLI](https://github.com/FisherRone/BiliNote-CLI)。使用前请参照 [BiliNote-CLI](https://github.com/FisherRone/BiliNote-CLI) 中的 `README.md` 完成安装和配置。

## 📦 安装本 Skill

```bash
npx skills add FisherRone/bilinote-cli-skill
```

- 或者直接将仓库中的 `bilinote-cli-skill`  文件夹复制到 Claude Code （或其他 agent）的 skills 目录。

## 🚀 使用

在 Claude Code 或任何支持 skill 的 Agent 中，直接说：

- `帮我总结这个视频 https://www.bilibili.com/video/BV1xx`
- `在 B 站搜一下“Python 入门”的教程，并给我笔记`
- `记笔记` + 粘贴一个链接

Agent 会自动调用 `bilinote process` 或 `bilinote search`，然后把生成的笔记交给你。

**自定义风格示例：**
```
用学术风格给这个视频做笔记，带截图和链接：
https://www.youtube.com/watch?v=xxx
```

## 📝 生成的笔记在哪

笔记默认输出到：

- macOS / Linux：`~/.bilinote/output/notes/`
- Windows：`C:\Users\<你的用户名>\.bilinote\output\notes\`

## 📖 更多

- BiliNote-CLI 完整文档：[GitHub 仓库](https://github.com/FisherRone/BiliNote-CLI)


## 📄 许可

MIT
