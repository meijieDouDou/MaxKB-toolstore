# Google Search

调用 Google Programmable Search Engine 的 Custom Search JSON API，返回网页搜索结果。

## 配置与调用

1. 创建 [Programmable Search Engine](https://programmablesearchengine.google.com/)，取得搜索引擎 ID `cx`，并申请 Custom Search API Key。
2. 从 MaxKB 工具商店添加工具，填写启动参数 `apikey` 与 `cx`，然后启用工具。
3. 在应用或工作流中传入 `query`，例如 `MaxKB documentation`。

| 参数 | 用途 |
| --- | --- |
| `apikey` | 启动参数，Google Custom Search API Key |
| `cx` | 启动参数，搜索引擎 ID |
| `query` | 必填输入，搜索关键词 |

工具返回 Google API 的 JSON 对象；请求失败时抛出异常。原内置工具代码固定请求最多 10 条结果。

## 版本

- 1.0.0：从 MaxKB 内置工具迁移，保留原有代码和参数。
