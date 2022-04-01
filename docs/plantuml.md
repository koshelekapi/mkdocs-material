# Диаграммы PlantUML

## build_plantuml

Ссылка: [https://pypi.org/project/mkdocs-build-plantuml-plugin/](https://pypi.org/project/mkdocs-build-plantuml-plugin/) 

Плагин работает с файлами PUML, содержащими исходный код диаграмм. Исходные файлы необходимо разместить в каталоге **docs/diagrams/src**.

Для включения диаграммы в статью необходимо в MD-файле статьи разместить ссылку на итоговый графический файл — после сборки он будет размещен в каталоге **diagrams/out**:

```
![file](diagrams/out/pay-api-payment01-ru.png)
```
Пример:

![file](diagrams/out/pay-api-payment01-ru.png)

##  plantuml-markdown

Ссылка: [https://github.com/mikitex70/plantuml-markdown](https://github.com/mikitex70/plantuml-markdown)

Этот плагин работает с исходным кодом диаграмм, который встроен непосредственно в MD-разметку статьи в виде:

    ```plantuml format="png" classes="uml myDiagram" alt="My super diagram placeholder" title="My super diagram" width="300px" height="300px"
      Goofy ->  MickeyMouse: calls
      Goofy <-- MickeyMouse: responds
    ```
Пример:

    ::uml:: format="png" classes="uml myDiagram" alt="My super diagram placeholder" title="My super diagram" width="300px" height="300px"
      Goofy ->  MickeyMouse: calls
      Goofy <-- MickeyMouse: responds
    ::end-uml::