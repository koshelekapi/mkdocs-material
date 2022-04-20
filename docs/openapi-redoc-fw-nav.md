---
hide:
  - toc
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

# OpenAPI — Redoc MD Fullwidth + Navigation

Пример встраивания документа Redoc на страницу MkDocs.

- [x] Скрыт блок оглавления (справа)
- [ ] Скрыт блок навигации (слева)
- [x] FW-режим с помощью CSS в статье

!!! example "Другие варианты представления:"

    [Redoc MD Base](openapi-redoc.md)
    
    [Redoc MD Wide](openapi-redoc-wide.md)
    
    [Redoc MD Fullwidth](openapi-redoc-fw.md)
    
    Redoc MD Fullwidth + Navigation (вы здесь)

---

<redoc spec-url='https://raw.githubusercontent.com/andwr/mkdocs-material-fork/main/docs/openapi/pay-api.yaml'></redoc>
<script src="https://cdn.jsdelivr.net/npm/redoc@latest/bundles/redoc.standalone.js"> 
</script>