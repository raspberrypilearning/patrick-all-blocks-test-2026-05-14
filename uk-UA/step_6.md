## Складаний

Збірні блоки (також звані панелями інгредієнтів) містять додатковий контент, такий як інструкції з встановлення або довідкові матеріали. Учні можуть розгортати або згортати панель за потреби.

---

### Знижка зі смаком малини

📖 [Специфікація RFM — Збірна](http://digital-docs.rpf-internal.org/docs/technology/codebases-and-products/raspberry-flavoured-markdown/specs/raspberry-flavoured-markdown-draft-spec#collapsible)

```markdown
> [!АККОРДЕОН] Як відкрити Thonny 
>
> Натисніть меню **Raspberry Pi**, потім **Програмування**, а потім **Thony Python IDE**.
```

> Як відкрити Тонні
>
> Натисніть меню **Raspberry Pi**, потім **Програмування**, а потім **Thonny Python IDE**.

---

### Спадщина Крамдаун РПФ

Для старого блоку `collapse` потрібен початковий розділ YAML з полем `title`. Тіло коду аналізується як Markdown.

**Просте згортання**

📖 [Специфікація Kramdown — Згорнути](http://digital-docs.rpf-internal.org/docs/technology/codebases-and-products/raspberry-flavoured-markdown/specs/kramdown_rpf-legacy-spec#collapse)

```markdown
---
заголовок: Як відкрити Thonny
---

Натисніть меню **Raspberry Pi**, потім **Програмування**, а потім **Thonny Python IDE**.

```

---

## назва: Як відкрити Тонні

Натисніть меню **Raspberry Pi**, потім **Програмування**, а потім **Thonny Python IDE**.

**Усередині елемента списку**

📖 [Специфікація Kramdown — Згорнути (всередині елемента списку)](http://digital-docs.rpf-internal.org/docs/technology/codebases-and-products/raspberry-flavoured-markdown/specs/kramdown_rpf-legacy-spec#inside-a-list-item)

````markdown
1. Відкрийте Thonny на вашому Raspberry Pi.

    ---
    заголовок: Відкриття Thonny
    ---

    Натисніть **меню Raspberry Pi > Програмування > Thonny Python IDE**.


1. Створіть новий файл і збережіть його як **weather.py**.

1. Додайте ваші імпортовані дані на початку файлу:

    ```python
    from sense_hat import SenseHat
    from time import sleep
```
````

1. Відкрийте Thonny на вашому Raspberry Pi.

   ---

   ## назва: Відкриття Тонні

   Натисніть **меню Raspberry Pi > Програмування > Thonny Python IDE**.

2. Створіть новий файл і збережіть його під назвою **weather.py**.

3. Додайте імпортовані дані на початку файлу:

    ```python
    from sense_hat import SenseHat
    from time import sleep
    ```
