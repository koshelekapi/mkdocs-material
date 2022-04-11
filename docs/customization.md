---
hide:
  - toc
  - navigation
---

# Кастомизация

## Additional CSS

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
## Переключение гаммы { #dark_theme }

Можно добавить переключатель светлой/темной темы (добавлена для примера на этом сайте).

## Отключение панелей навигации { #page_layout }

На каждой странице поддерживается возможность отключения панелей навигации слева и справа. 
На данной странице для примера отключена панель справа (оглавление страницы).