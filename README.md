# 繁转简与排版

一个面向 ChatGPT 与 Codex 的纯技能插件，用于：

- 将繁体中文按上下文转换为简体中文；
- 整理中文标点、空格、段落、标题、列表与 Markdown；
- 保护代码、命令、链接、路径、版本号和专有名词；
- 默认只输出处理后的正文，不擅自改写原意。

## 安装

将本仓库添加为 Codex 插件 marketplace：

```powershell
codex plugin marketplace add RedScarf777/new
```

然后在 ChatGPT 桌面端或 Codex 的 Plugins Directory 中，从“RedScarf777 中文工具”来源安装“繁转简与排版”。安装或更新后重启桌面端。

## 使用示例

```text
把下面的繁体中文转成简体并整理排版：

我們正在開發一個軟體工具，它支援 Markdown、API 文件與程式碼範例。
```

也可以明确限制处理范围：

```text
只做繁简转换和标点整理，不改词、不润色；代码块保持原样。
```

## 结构

- `plugin.json`：便携式插件清单；
- `skills/zh-hans-polisher/SKILL.md`：转换和排版规则；
- `.agents/plugins/marketplace.json`：从本 GitHub 仓库安装时使用的 marketplace 清单。

## 隐私

这是一个不包含 MCP 服务的纯技能插件，不需要 API key，也不会自行把文本发送到第三方服务。

## 许可证

MIT

