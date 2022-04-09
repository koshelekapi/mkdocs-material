# Разметка

> Источник: [https://squidfunk.github.io/mkdocs-material/setup/extensions/python-markdown-extensions/](https://squidfunk.github.io/mkdocs-material/setup/extensions/python-markdown-extensions/)

Поддерживается базовая разметка Markdown, которую можно расширить подключением [плагинов](plugins.md) (например, если нужны вкладки). В частности, плагин Pymdown Extensions предлагает следующую коллекцию расширений:

[https://facelessuser.github.io/pymdown-extensions/#extensions](https://facelessuser.github.io/pymdown-extensions/#extensions)

---

# Заголовок 1

## Заголовок 2

### Заголовок 3

#### Заголовок 4

##### Заголовок 5

###### Заголовок 6

Plain text 

**bold** 

_italic_

~strikethrough~

`monospace`

**`monospace bold`**

# `monospace h1`

---

1. One
2. Two
3. Three


* list item level 1
   * list item level 2
      * list item level 3
         * list item level 4
            * etc


> Цитата

---

!!! tip Use the language switcher in the header to switch between the localized versions of this demo website. This switcher is part of mkdocs-material >= 7.1.0 and is automatically configured by this plugin or can be statically configured from the mkdocs.yml file.

---

| Prop | Type | Required | Default | Description |
| ---- |:----:|:---:|:-------:| :----------:|
| type | `String` |`N`| `errorPage`|`errorPage`, `noNetwork`, `noGoods`, `errorLocation`|
| show | `Boolean` |`N`| `true` | whether to show |
| padding-top | `Number` |`N`| `240` | padding top from screen |
| custom-set | `Object` |`N`| `{}` |custom config [type.js](https://github.com/apache/incubator-weex-ui/blob/master/packages/wxc-result/type.js)|
| wrap-style | `Object` | `N`|`{}` | custom wrap style|

```json
{
   "card": { // карта лояльности пользователя
      "cardNumber": "", // номер карты в информационной системе партнера
      "cardState" : "", // состояние карты ("active" / "inactive")
      "barcode": { // штрихкод карты
         "barcodeNumber": 1234567890, // номер штрихкода
         "barcodeType": ""    // тип штрихкода ("EAN_8" / "EAN_13" / "CODE_128" / "UPC_A" / "QR_CODE")
    }
  }
}
```

=== "Tab-01"
    notice with `inline code` and additional placeholder text used
    to force the content to wrap and span multiple lines.

=== "Tab-02"
    ```
    notice with `inline code` and additional placeholder text used
    to force the content to wrap and span multiple lines.
    ```

    | Prop | Type | Required | Default | Description |
    | ---- |:----:|:---:|:-------:| :----------:|
    | type | `String` |`N`| `errorPage`|`errorPage`, `noNetwork`, `noGoods`, `errorLocation`|
    | show | `Boolean` |`N`| `true` | whether to show |
    | padding-top | `Number` |`N`| `240` | padding top from screen |
    | custom-set | `Object` |`N`| `{}` |custom config [type.js](https://github.com/apache/incubator-weex-ui/blob/master/packages/wxc-result/type.js)|
    | wrap-style | `Object` | `N`|`{}` | custom wrap style|

![jpg](assets/jpg.jpg)

![gif](assets/gif.gif)

