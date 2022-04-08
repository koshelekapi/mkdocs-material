# Разметка

> Источник: [https://squidfunk.github.io/mkdocs-material/setup/extensions/python-markdown-extensions/](https://squidfunk.github.io/mkdocs-material/setup/extensions/python-markdown-extensions/)

Поддерживается базовая разметка Markdown, которую можно сконфигурировать или расширить подключением [плагинов](plugins.md) (например, если нужны вкладки).

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

* bullet level 1
   * bullet level 2
      * bullet level 3
         * bullet level 4
            * etc


> Цитата

!> **Important** notice with `inline code` and additional placeholder text used
to force the content to wrap and span multiple lines.

?> **Tip** notice with `inline code` and additional placeholder text used to
force the content to wrap and span multiple lines.

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
         "barcodeNumber": "", // номер штрихкода
         "barcodeType": ""    // тип штрихкода ("EAN_8" / "EAN_13" / "CODE_128" / "UPC_A" / "QR_CODE")
    }
  }
}
```

=== "Tab 1"
    Markdown **content**.

    Multiple paragraphs.

=== "Tab 2"
    More Markdown **content**.

    - list item a
    - list item b


=== "Tab-01"
!> **Important** notice with `inline code` and additional placeholder text used
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
