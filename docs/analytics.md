> Источник: [https://squidfunk.github.io/mkdocs-material/setup/setting-up-site-analytics/](https://squidfunk.github.io/mkdocs-material/setup/setting-up-site-analytics/)

Поддерживается интеграция с Google Analytics и Universal Analytics. 
Для включения GA необходимо добавить следующие строки в файл конфигурации **mkdocs.yml**:

```
extra:
  analytics:
    provider: google
    property: G-XXXXXXXXXX

```

??? question "How to measure site search usage?"

    Besides page views and events, site search can be tracked to better
    understand how people use your documentation and what they expect to find.
    In order to enable site search tracking, the following steps are required:

    === ":material-google-analytics: Google Analytics 4"

        1. Go to your Google Analytics __admin settings__
        2. Select the property for the respective tracking code
        3. Select the __data streams__ tab and click the corresponding URL
        4. Click the gear icon within the __enhanced measurement__ section
        5. Ensure that __site search__ is enabled

    === ":material-google-analytics: Universal Analytics"

        1.  Go to your Google Analytics __admin settings__
        2.  Select the property for the respective tracking code
        3.  Go to the __view settings__ tab
        4.  Scroll down and enable __site search settings__
        5.  Set the __query parameter__ to `q`