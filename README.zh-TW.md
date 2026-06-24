# 🔍 OpenAPI Viewer

在瀏覽器中直接渲染任何 OpenAPI/Swagger 規格——無需安裝、無需後端。

[![Demo](https://img.shields.io/badge/demo-GitHub%20Pages-blue)](https://min0625.github.io/openapi-viewer/)
[![Swagger UI](https://img.shields.io/badge/Swagger%20UI-5.30.2-green)](https://github.com/swagger-api/swagger-ui)
[![License](https://img.shields.io/badge/license-MIT-blue.svg)](LICENSE)

繁體中文 | [English](./README.md)

## 使用方式

在 URL 後加上 `?url=` 參數，指向任何公開的 OpenAPI/Swagger JSON 或 YAML 檔案：

```
https://min0625.github.io/openapi-viewer/?url=https://petstore3.swagger.io/api/v3/openapi.json
```

不帶 `?url=` 直接訪問會載入預設範例文件。Explore 欄位在切換規格時會同步更新 `?url=`，讓每份文件都有可加書籤、可分享的網址。

支援 Swagger 2.0、OpenAPI 3.0.x 及 OpenAPI 3.1.x，格式為 JSON 或 YAML。僅接受 `http(s)` 與同源網址。

## 範例

[`examples/`](examples/) 提供一組範例規格——同一個 Users API 以各版本／格式撰寫：

| 版本 | JSON | YAML |
| --- | --- | --- |
| Swagger 2.0 | [`swagger-2.0.json`](examples/swagger-2.0.json) · [開啟](https://min0625.github.io/openapi-viewer/?url=examples/swagger-2.0.json) | [`swagger-2.0.yaml`](examples/swagger-2.0.yaml) · [開啟](https://min0625.github.io/openapi-viewer/?url=examples/swagger-2.0.yaml) |
| OpenAPI 3.0 | [`openapi-3.0.json`](examples/openapi-3.0.json) · [開啟](https://min0625.github.io/openapi-viewer/?url=examples/openapi-3.0.json) | [`openapi-3.0.yaml`](examples/openapi-3.0.yaml) · [開啟](https://min0625.github.io/openapi-viewer/?url=examples/openapi-3.0.yaml) |
| OpenAPI 3.1 | [`openapi-3.1.json`](examples/openapi-3.1.json) · [開啟](https://min0625.github.io/openapi-viewer/?url=examples/openapi-3.1.json) | [`openapi-3.1.yaml`](examples/openapi-3.1.yaml) · [開啟](https://min0625.github.io/openapi-viewer/?url=examples/openapi-3.1.yaml) |

## CORS

載入的規格網址必須允許跨域請求。GitHub Raw 與 Gist 網址不受 CORS 限制：

```
https://raw.githubusercontent.com/<user>/<repo>/<branch>/<path>
https://gist.githubusercontent.com/<user>/<gist-id>/raw/<file>
```

## 授權

MIT — 詳見 [LICENSE](LICENSE)
