# 🔍 OpenAPI Viewer

A simple and elegant OpenAPI/Swagger documentation viewer hosted on GitHub Pages. Supports dynamic loading of any public API specification files.

[![GitHub Pages](https://img.shields.io/badge/demo-GitHub%20Pages-blue)](https://min0625.github.io/openapi-viewer/)
[![Swagger UI](https://img.shields.io/badge/Swagger%20UI-5.10.0-green)](https://github.com/swagger-api/swagger-ui)
[![License](https://img.shields.io/badge/license-MIT-blue.svg)](LICENSE)

[繁體中文](./README.zh-TW.md) | English

## ✨ Features

- 🎯 **Multi-Version Support**: Compatible with both Swagger 2.0 and OpenAPI 3.x specifications
- 🔗 **Dynamic Loading**: Load any public API documentation via URL parameters
- 🎨 **Real-time Rendering**: Render documentation using official Swagger UI
- 🚀 **Zero Deployment**: Powered by GitHub Pages with zero configuration
- 📱 **Responsive Design**: Works seamlessly across all device screen sizes
- ⚡ **Auto Detection**: Automatically identifies and displays API specification versions
- 🛡️ **Error Handling**: User-friendly error messages and feedback

## 🚀 Quick Start

### Method 1: Load External API Documentation

Add the `?uri=` parameter to the URL, pointing to your OpenAPI/Swagger JSON file:

```
https://min0625.github.io/openapi-viewer?uri=https://petstore3.swagger.io/api/v3/openapi.json
```

### Method 2: Load Files from GitHub

Use GitHub Raw URL:

```
https://min0625.github.io/openapi-viewer?uri=https://raw.githubusercontent.com/username/repo/main/openapi.json
```

### Method 3: No URI Parameter

If you visit without the `uri` parameter, you'll see a helpful guide on how to use the viewer.

## 📚 Usage Examples

### Swagger 2.0 Example
```
https://min0625.github.io/openapi-viewer?uri=https://petstore.swagger.io/v2/swagger.json
```

### OpenAPI 3.0 Example
```
https://min0625.github.io/openapi-viewer?uri=https://petstore3.swagger.io/api/v3/openapi.json
```

### Load from Private Gist
```
https://min0625.github.io/openapi-viewer?uri=https://gist.githubusercontent.com/username/gist-id/raw/openapi.json
```

## 🛠️ Technical Specifications

- **Swagger UI**: v5.10.0
- **Supported Formats**: 
  - Swagger 2.0 (JSON/YAML)
  - OpenAPI 3.0.x (JSON/YAML)
  - OpenAPI 3.1.x (JSON/YAML)
- **Browser Support**: All modern browsers (Chrome, Firefox, Safari, Edge)

## 📦 Local Development

### 1. Clone the Project
```bash
git clone https://github.com/min0625/openapi-viewer.git
cd openapi-viewer
```

### 2. Start Local Server
```bash
# Using Python
python -m http.server 8000

# Or using Node.js
npx serve .
```

### 3. View Documentation
Open your browser and visit `http://localhost:8000`

## 🔧 Customization

You can fork this project and modify `index.html` to:

- Adjust UI theme colors
- Add custom CSS styles
- Change default loading behavior
- Add additional Swagger UI configurations

## ⚠️ Important Notes

### CORS Limitations
The loaded API documentation must allow cross-origin requests (CORS). If you encounter CORS errors:

1. Ensure the target server has proper CORS headers configured
2. Use GitHub Raw URLs or GitHub Gist
3. Use CORS-enabled CDN services

### GitHub Raw URL Format
When using GitHub files, use the following format:
```
https://raw.githubusercontent.com/<user>/<repo>/<branch>/<path-to-file>
```

## 🤝 Contributing

Issues and Pull Requests are welcome!

1. Fork this project
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details

## 🙏 Acknowledgments

- [Swagger UI](https://github.com/swagger-api/swagger-ui) - Providing excellent API documentation viewing tools
- [OpenAPI Initiative](https://www.openapis.org/) - Maintaining the OpenAPI specification standards

## 📮 Contact

If you have any questions or suggestions:

- Open an Issue: [GitHub Issues](https://github.com/min0625/openapi-viewer/issues)
- Contact Author: [@min0625](https://github.com/min0625)

---

<p align="center">Made with ❤️ by <a href="https://github.com/min0625">Min Huang</a></p>