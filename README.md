# 🔍 OpenAPI Viewer

Render any OpenAPI/Swagger spec in your browser — no installation, no backend.

[![Demo](https://img.shields.io/badge/demo-GitHub%20Pages-blue)](https://min0625.github.io/openapi-viewer/)
[![Swagger UI](https://img.shields.io/badge/Swagger%20UI-5.30.2-green)](https://github.com/swagger-api/swagger-ui)
[![License](https://img.shields.io/badge/license-MIT-blue.svg)](LICENSE)

[繁體中文](./README.zh-TW.md) | English

## Usage

Pass any public OpenAPI/Swagger JSON or YAML URL via `?url=`:

```
https://min0625.github.io/openapi-viewer/?url=https://petstore3.swagger.io/api/v3/openapi.json
```

Visiting without `?url=` loads the bundled default spec. The Explore box updates `?url=` on navigation, so every spec has a shareable, bookmarkable URL.

Supports Swagger 2.0, OpenAPI 3.0.x, and OpenAPI 3.1.x — JSON or YAML. Only `http(s)` and same-origin URLs are accepted.

## Examples

Bundled specs under [`examples/`](examples/) — the same Users API across all supported versions:

| Version | JSON | YAML |
| --- | --- | --- |
| Swagger 2.0 | [`swagger-2.0.json`](examples/swagger-2.0.json) · [open](https://min0625.github.io/openapi-viewer/?url=examples/swagger-2.0.json) | [`swagger-2.0.yaml`](examples/swagger-2.0.yaml) · [open](https://min0625.github.io/openapi-viewer/?url=examples/swagger-2.0.yaml) |
| OpenAPI 3.0 | [`openapi-3.0.json`](examples/openapi-3.0.json) · [open](https://min0625.github.io/openapi-viewer/?url=examples/openapi-3.0.json) | [`openapi-3.0.yaml`](examples/openapi-3.0.yaml) · [open](https://min0625.github.io/openapi-viewer/?url=examples/openapi-3.0.yaml) |
| OpenAPI 3.1 | [`openapi-3.1.json`](examples/openapi-3.1.json) · [open](https://min0625.github.io/openapi-viewer/?url=examples/openapi-3.1.json) | [`openapi-3.1.yaml`](examples/openapi-3.1.yaml) · [open](https://min0625.github.io/openapi-viewer/?url=examples/openapi-3.1.yaml) |

## CORS

The spec URL must allow cross-origin requests. GitHub Raw and Gist URLs work without CORS restrictions:

```
https://raw.githubusercontent.com/<user>/<repo>/<branch>/<path>
https://gist.githubusercontent.com/<user>/<gist-id>/raw/<file>
```

## License

MIT — see [LICENSE](LICENSE)
