# 🔍 OpenAPI Viewer

一個簡潔優雅的 OpenAPI/Swagger 文件檢視器,透過 GitHub Pages 託管,支援動態載入任何公開的 API 規格文件。

[![GitHub Pages](https://img.shields.io/badge/demo-GitHub%20Pages-blue)](https://min0625.github.io/openapi-viewer/)
[![Swagger UI](https://img.shields.io/badge/Swagger%20UI-5.10.0-green)](https://github.com/swagger-api/swagger-ui)
[![License](https://img.shields.io/badge/license-MIT-blue.svg)](LICENSE)

繁體中文 | [English](./README.md)

## ✨ 特色功能

- 🎯 **支援多版本**: 同時支援 Swagger 2.0 和 OpenAPI 3.x 規格
- 🔗 **動態載入**: 透過 URL 參數載入任何公開的 API 文件
- 🎨 **即時渲染**: 使用官方 Swagger UI 進行文件渲染
- 🚀 **無需部署**: 直接使用 GitHub Pages,零設定
- 📱 **響應式設計**: 支援各種裝置螢幕尺寸
- ⚡ **自動檢測**: 自動識別並顯示 API 規格版本
- 🛡️ **錯誤處理**: 友善的錯誤訊息提示

## 🚀 快速開始

### 方式 1: 載入外部 API 文件

在 URL 後加上 `?uri=` 參數,指向你的 OpenAPI/Swagger JSON 檔案:

```
https://min0625.github.io/openapi-viewer?uri=https://petstore3.swagger.io/api/v3/openapi.json
```

### 方式 2: 載入 GitHub 上的檔案

使用 GitHub Raw URL:

```
https://min0625.github.io/openapi-viewer?uri=https://raw.githubusercontent.com/username/repo/main/openapi.json
```

### 方式 3: 不提供 URI 參數

如果直接訪問而不帶 `uri` 參數,會顯示使用說明引導頁面。

## 📚 使用範例

### Swagger 2.0 範例
```
https://min0625.github.io/openapi-viewer?uri=https://petstore.swagger.io/v2/swagger.json
```

### OpenAPI 3.0 範例
```
https://min0625.github.io/openapi-viewer?uri=https://petstore3.swagger.io/api/v3/openapi.json
```

### 載入私有 Gist
```
https://min0625.github.io/openapi-viewer?uri=https://gist.githubusercontent.com/username/gist-id/raw/openapi.json
```

## 🛠️ 技術規格

- **Swagger UI**: v5.10.0
- **支援格式**: 
  - Swagger 2.0 (JSON/YAML)
  - OpenAPI 3.0.x (JSON/YAML)
  - OpenAPI 3.1.x (JSON/YAML)
- **瀏覽器支援**: 所有現代瀏覽器 (Chrome, Firefox, Safari, Edge)

## 📦 本地開發

### 1. Clone 專案
```bash
git clone https://github.com/min0625/openapi-viewer.git
cd openapi-viewer
```

### 2. 啟動本地伺服器
```bash
# 使用 Python
python -m http.server 8000

# 或使用 Node.js
npx serve .
```

### 3. 瀏覽文件
開啟瀏覽器訪問 `http://localhost:8000`

## 🔧 自訂設定

你可以 Fork 這個專案並修改 `index.html` 來:

- 調整 UI 主題顏色
- 新增自訂 CSS 樣式
- 修改預設載入行為
- 新增額外的 Swagger UI 設定

## ⚠️ 注意事項

### CORS 限制
載入的 API 文件必須允許跨域請求 (CORS)。如果遇到 CORS 錯誤:

1. 確保目標伺服器設定了正確的 CORS headers
2. 使用 GitHub Raw URL 或 GitHub Gist
3. 使用支援 CORS 的 CDN 服務

### GitHub Raw URL 格式
使用 GitHub 檔案時,使用以下格式:
```
https://raw.githubusercontent.com/<user>/<repo>/<branch>/<path-to-file>
```

## 🤝 貢獻

歡迎提交 Issue 或 Pull Request!

1. Fork 這個專案
2. 建立你的功能分支 (`git checkout -b feature/AmazingFeature`)
3. 提交你的變更 (`git commit -m 'Add some AmazingFeature'`)
4. 推送到分支 (`git push origin feature/AmazingFeature`)
5. 開啟一個 Pull Request

## 📄 授權

本專案採用 MIT 授權條款 - 詳見 [LICENSE](LICENSE) 檔案

## 🙏 致謝

- [Swagger UI](https://github.com/swagger-api/swagger-ui) - 提供優秀的 API 文件檢視工具
- [OpenAPI Initiative](https://www.openapis.org/) - 維護 OpenAPI 規格標準

## 📮 聯絡方式

如有任何問題或建議,歡迎:

- 開Issue: [GitHub Issues](https://github.com/min0625/openapi-viewer/issues)
- 聯絡作者: [@min0625](https://github.com/min0625)

---

<p align="center">Made with ❤️ by <a href="https://github.com/min0625">Min Huang</a></p>