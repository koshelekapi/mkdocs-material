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

```plantuml format="png"
autonumber "<font color=red><b>[00]"
actor Пользователь as User
box Кошелёк #plum
	participant "Приложение\nКошелёк" as Wallet
	participant "Сервер\nКошелёк Pay API" as CMPAY 
end box
box Партнёр #lightblue 
	participant "Касса и ЦОД ТСП" as POS
end box

User->POS: Выкладка товаров к покупке
User->Wallet: Выбор карты лояльности в Кошельке
Wallet->POS: Штрихкод карты лояльности
POS->POS: - Сканирование товаров.\n- Считывание из Кошелька номера карты лояльности. \n- Проверка доступности оплаты через Кошелёк Pay\n (в ШК содержится //cardSession//). \n- Валидация парольной части. \n- Идентификация покупателя по //loyaltyId//.\n- Расчет суммы.  

POS->POS: Кассир выполняет закрытие чека на кассе
alt ШК содержит //cardSession//
POS->CMPAY: <back:gold>**[Кошелёк Pay API]**</back> **POST** /availability-info/task\nЗапрос списка возможных провайдеров платежей
alt HTTP Status Code = 200
 CMPAY-->POS: Список провайдеров платежей
else HTTP Status Code = 201
CMPAY-->POS: //availabilityInfoId, timeout//
loop Запрос списка провайдеров платежей до получения результата
POS->CMPAY: <back:gold>**[Кошелёк Pay API]**</back> **GET** /availability-info/{availabilityInfoId}\nПолучение списка доступных провайдеров платежей
CMPAY-->POS: Список провайдеров платежей
end loop

end
else ШК не содержит //cardSession//
POS->POS: Оплата "Кошелёк Pay"\nне подключена у покупателя
note over POS
Стандартный сценарий оплаты (карта, наличные)
end note
end

opt#Gold #LightBlue Расчет скидок и бонусов
POS->POS: Обращение к ЦОД ТСП\nдля расчета скидок и бонусов 
POS->POS: Получение скидок и\nбонусов от ЦОД ТСП
POS->POS: Формирование итоговой\nсуммы платежа
end
```