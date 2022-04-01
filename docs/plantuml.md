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