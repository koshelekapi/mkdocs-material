---
hide:
  - toc
  - navigation
---

# OpenAPI — Stoplight

Пример встраивания документа Stoplight на страницу MkDocs приведен ниже.

---

<script src="https://unpkg.com/@stoplight/elements/web-components.min.js">
  </script>
<link rel="stylesheet" href="https://unpkg.com/@stoplight/elements/styles.min.css">
<elements-api
      apiDescriptionUrl="https://raw.githubusercontent.com/andwr/mkdocs-material-fork/main/docs/openapi/pay-api.yaml"
      router="hash"
    />