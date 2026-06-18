## Блоки коду Microbit та Scratch

Обгороджені блоки коду зі спеціалізованими мовними ідентифікаторами відображаються з відповідними CSS-класами, які підхоплюються інтерактивними віджетами на сторінці.

---

### Блок мікробітного коду

Обгороджений блок коду з ідентифікатором мови `microbit` відтворюється з використанням `class="language-microbit"`, який використовує віджет симулятора BBC micro:bit для відображення інтерактивного попереднього перегляду.

📖 [Специфікація Kramdown — блок мікробітного коду](http://digital-docs.rpf-internal.org/docs/technology/codebases-and-products/raspberry-flavoured-markdown/specs/kramdown_rpf-legacy-spec#microbit-code-block)

````markdown
```мікробіт
з імпорту мікробітів *

поки True:
    display.show(Image.HEART)
    sleep(1000)
    display.clear()
    sleep(1000)
```
````

```microbit
з імпорту мікробітів *

поки True:
    display.show(Image.HEART)
    sleep(1000)
    display.clear()
    sleep(1000)
```

---

### Блоки скретч-коду

Блоки коду, огороджені мовою `blocks3` (Scratch 3) або `blocks` (Scratch 2), відображаються з відповідним класом CSS. Бібліотека рендерингу scratchblocks використовує ці класи для малювання візуальних представлень блоків Scratch.

**Скретч 3 (`блоки3`)**

📖 [Специфікація Kramdown — блоки скретч-коду](http://digital-docs.rpf-internal.org/docs/technology/codebases-and-products/raspberry-flavoured-markdown/specs/kramdown_rpf-legacy-spec#scratch-code-blocks)

````markdown
```блоки3
коли натиснуто прапорець
повторити (10)
  перемістити (10) кроки
кінець
```
````

```blocks3
коли натиснуто прапорець
повторити (10)
  перемістити (10) кроки
кінець
```

**Скретч 2 (`блоки`)**

````markdown
```блоки
при натисканні прапорця
повтор (10)
  переміщення (10) кроків
```
````

```blocks
коли натиснуто прапорець
повторити (10)
  перемістити (10) кроків
```

***
Цей проєкт переклали волонтери:

[name]

[name]

[name]

Завдяки волонтерам ми надаємо можливість людям у всьому світі навчатися рідною мовою. Ви також можете допомогти нам у цьому — більше інформації про волонтерську програму на [rpf.io/translate](https://rpf.io/translate).
