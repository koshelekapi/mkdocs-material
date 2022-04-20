---
hide:
  - toc
  - navigation
---

<style>
@media only screen and (min-width: 76.25em) {
  .md-main__inner {
    max-width: none;
  }
  .md-sidebar--primary {
    left: 0;
  }
  .md-sidebar--secondary {
    right: 0;
    margin-left: 0;
    -webkit-transform: none;
    transform: none;   
  }
}
</style>

# OpenAPI — Redoc

Пример встраивания документа Redoc на страницу MkDocs.

- [x] Скрыт блок оглавления (справа)
- [x] Скрыт блок навигации (слева)
- [x] FW-режим с помощью CSS в статье

[Перейти к следующему представлению](openapi-redoc-fw-nav.md)

---

<redoc spec-url='https://raw.githubusercontent.com/andwr/mkdocs-material-fork/main/docs/openapi/pay-api.yaml'></redoc>
<script src="https://cdn.jsdelivr.net/npm/redoc@latest/bundles/redoc.standalone.js"> 
</script>