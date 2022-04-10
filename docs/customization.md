# Кастомизация

> Источник: [https://squidfunk.github.io/mkdocs-material/customization/#additional-css](https://squidfunk.github.io/mkdocs-material/customization/#additional-css)

Настройка внешнего вида сайта выполняется на уровне файла **extra.css**. Файл необходимо разместить в каталоге **docs/stylesheets**:

```
.
├─ docs/
│  └─ stylesheets/
│     └─ extra.css
└─ mkdocs.yml
```

Затем необходимо указать на него в файле **mkdocs.yml**:

```
extra_css:
  - stylesheets/extra.css

```

Можно добавить переключатель светлой/темной темы (добавлена для примера на этом сайте).