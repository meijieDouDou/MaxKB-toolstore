# LangSearch

调用 LangSearch Web Search API，以自然语言问题检索网页并返回 API 的 JSON 响应。

## 配置与调用

1. 在 [LangSearch](https://langsearch.com/) 申请 API Key。
2. 从 MaxKB 工具商店添加工具，在启动参数 `apikey` 中填写密钥，然后启用工具。
3. 在应用或工作流中传入 `query`，例如 `人工智能行业动态`。

| 参数 | 用途 |
| --- | --- |
| `apikey` | 启动参数，LangSearch API Key |
| `query` | 必填输入，搜索问题或关键词 |

工具返回 LangSearch API 的 JSON 对象；请求失败时抛出异常。原内置工具代码启用摘要和实时抓取，固定请求 20 条结果。

## 版本

- 1.0.0：从 MaxKB 内置工具迁移，保留原有代码和参数。
