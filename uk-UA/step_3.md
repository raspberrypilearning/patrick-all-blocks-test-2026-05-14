## Завдання

Блоки завдань огортають окрему одиницю роботи. Вони відображаються з прапорцем, який учні можуть поставити після завершення кроку. Завдання можуть містити код, підказки та панелі, що розгортаються.

---

### Знижка зі смаком малини

📖 [Специфікація RFM — Завдання](http://digital-docs.rpf-internal.org/docs/technology/codebases-and-products/raspberry-flavoured-markdown/specs/raspberry-flavoured-markdown-draft-spec#task)

```markdown
> [!ЗАВДАННЯ]
>
> Виконайте цей крок.
```

> Виконайте цей крок.

---

### Спадщина Крамдаун РПФ

Базове завдання, що містить код та прозу.

📖 [Специфікація Крамдауна — Завдання](http://digital-docs.rpf-internal.org/docs/technology/codebases-and-products/raspberry-flavoured-markdown/specs/kramdown_rpf-legacy-spec#task)

````markdown

Додайте ключове слово `global`, щоб функція могла оновлювати змінну `temperature`:

```python
def update_display(event):
    глобальна температура
```

Тепер ви можете читати та записувати `temperature` зсередини `update_display`.

````

Додайте ключове слово `global`, щоб функція могла оновлювати змінну `temperature`:

```python
def update_display(подія):
    глобальна температура
```

Тепер ви можете читати та записувати `temperature` зсередини `update_display`.

#### З підказками

Завдання можуть містити блок «підказок», щоб надати учням додаткову допомогу, не захаращуючи основний крок.

📖 [Специфікація Крамдауна — Завдання (з підказками)](http://digital-docs.rpf-internal.org/docs/technology/codebases-and-products/raspberry-flavoured-markdown/specs/kramdown_rpf-legacy-spec#with-hints)

```markdown

Зчитайте поточну температуру та відобразіть її на світлодіодній матриці Sense HAT.


Підказка 1: Викличте `sense.get_temperature()`, щоб зчитати температуру.


Підказка 2: Збережіть результат: `temperature = sense.get_temperature()`


Підказка 3: Відобразіть його за допомогою `sense.show_message(str(round(temperature, 1)))`.


```

Зчитуйте поточну температуру та відображайте її на світлодіодній матриці Sense HAT.

Підказка 1: Викличте `sense.get_temperature()`, щоб зчитати температуру.

Підказка 2: Збережіть результат: `temperature = sense.get_temperature()`

Підказка 3: Відобразіть це за допомогою `sense.show_message(str(round(temperature, 1)))`.

#### Зі складним інгредієнтом

Завдання також можуть містити блок `collapse` для вбудовування вмісту інгредієнтів.

📖 [Специфікація Крамдауна — Завдання (з інгредієнтом)](http://digital-docs.rpf-internal.org/docs/technology/codebases-and-products/raspberry-flavoured-markdown/specs/kramdown_rpf-legacy-spec#with-ingredient)

````markdown

Налаштуйте Raspberry Pi та встановіть необхідне програмне забезпечення.

---
заголовок: Як встановити бібліотеку Sense HAT
---

Відкрийте термінал та виконайте:

```bash
pip install sense-hat
```

Перезавантажте Raspberry Pi після встановлення.


````

Налаштуйте Raspberry Pi та встановіть необхідне програмне забезпечення.

---

## заголовок: Як встановити бібліотеку Sense HAT

Відкрийте термінал і виконайте команду:

```bash
pip встановити sense-hat
```

Перезавантажте Raspberry Pi після встановлення.


