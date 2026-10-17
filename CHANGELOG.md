# Changelog

## 1.0.0

- 新增 `deepseek_search` 工具，调用 DeepSeek `/v1/tools/search`，默认返回 4 条摘要。
- 新增 `deepseek_fetch` 工具，调用 DeepSeek `/v1/tools/fetch` 抓取网页 Markdown 正文。
- 支持结果缓存、Search / Fetch 独立限速、408/429/5xx 重试和超时控制。
- API Key 仅从插件配置 `[provider].api_key` 读取。
- 工具通过 `visibility="visible"` 直接暴露给模型，无需 `tool_search` 发现。
- WebUI 配置项增加中文标签和说明，配置版本改为只读展示。
