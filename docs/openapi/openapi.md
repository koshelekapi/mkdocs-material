# OpenAPI

## mkdocs-render-swagger-plugin

> Источник: [https://pypi.org/project/mkdocs-render-swagger-plugin/](https://pypi.org/project/mkdocs-render-swagger-plugin/)

Плагин обрабатывает локальный файл OAS в формате JSON или YAML. Для рендеринга используется [Swagger UI](https://swagger.io/tools/swagger-ui/).

Пример Pay API:

!!swagger pay-api.yaml!!

<html lang="en">
  <head>
    <meta charset="utf-8">
    <meta name="viewport" content="width=device-width, initial-scale=1, shrink-to-fit=no">
    <title>Elements in HTML</title>
    <!-- Embed elements Elements via Web Component -->
    <script src="https://unpkg.com/@stoplight/elements/web-components.min.js"></script>
    <link rel="stylesheet" href="https://unpkg.com/@stoplight/elements/styles.min.css">
  </head>
  <body>

    <elements-api
      apiDescriptionUrl="https://api.apis.guru/v2/specs/github.com/1.1.4/openapi.yaml"
      router="hash"
      layout="sidebar"
    />

  </body>
</html>