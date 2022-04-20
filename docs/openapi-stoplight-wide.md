---
hide:
  - toc
  - navigation
---

# Stoplight MD Wide

Пример встраивания документа Stoplight на страницу MkDocs.

!!! example "Варианты представления (рекомендуется просмотр на подключенном дисплее):"

    [Stoplight MD Base](openapi-stoplight.md)
    
    Stoplight MD Wide (вы здесь)
    
    [Stoplight MD Fullwidth](openapi-stoplight-fw.md)
    
    [Stoplight MD Fullwidth + Navigation](openapi-stoplight-fw-nav.md)

- [x] Скрыт блок оглавления (справа)
- [x] Скрыт блок навигации (слева)
- [ ] FW-режим с помощью CSS в статье

---

<script src="https://unpkg.com/@stoplight/elements/web-components.min.js">
  </script>
<link rel="stylesheet" href="https://unpkg.com/@stoplight/elements/styles.min.css">
<elements-api
      apiDescriptionUrl="https://raw.githubusercontent.com/andwr/mkdocs-material-fork/main/docs/openapi/pay-api.yaml"
      router="hash"
    />
