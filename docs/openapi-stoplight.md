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
