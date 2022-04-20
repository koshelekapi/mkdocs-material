---
hide:
  - toc
---

# OpenAPI — Redoc (MD)

Пример встраивания документа Redoc на страницу MkDocs.

- [x] Скрыт блок оглавления (справа)
- [ ] Скрыт блок навигации (слева)
- [ ] FW-режим с помощью CSS в статье

!!! example "Другие варианты представления:"

  Redoc MD Base (вы здесь)
  
  [Redoc MD Wide](openapi-redoc-wide.md)
  
  [Redoc MD Fullwidth](openapi-redoc-fw.md)
  
  [Redoc MD Fullwidth + Navigation](openapi-redoc-fw-nav.md)

---

<redoc spec-url='https://raw.githubusercontent.com/andwr/mkdocs-material-fork/main/docs/openapi/pay-api.yaml'></redoc>
<script src="https://cdn.jsdelivr.net/npm/redoc@latest/bundles/redoc.standalone.js"> 
</script>