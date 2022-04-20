---
hide:
  - toc
  - navigation
---

# Redoc MD Wide

Пример встраивания документа Redoc на страницу MkDocs.

!!! example "Варианты представления (рекомендуется просмотр на подключенном дисплее):"

    [Redoc MD Base](openapi-redoc.md)
    
    Redoc MD Wide (вы здесь)
    
    [Redoc MD Fullwidth](openapi-redoc-fw.md)
    
    [Redoc MD Fullwidth + Navigation](openapi-redoc-fw-nav.md)

- [x] Скрыт блок оглавления (справа)
- [x] Скрыт блок навигации (слева)
- [ ] FW-режим с помощью CSS в статье

---

<redoc spec-url='https://raw.githubusercontent.com/andwr/mkdocs-material-fork/main/docs/openapi/pay-api.yaml'></redoc>
<script src="https://cdn.jsdelivr.net/npm/redoc@latest/bundles/redoc.standalone.js"> 
</script>