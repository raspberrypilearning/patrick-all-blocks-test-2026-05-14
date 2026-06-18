## Без друку, лише друк та розрив сторінки

Ці три блоки контролюють, як контент відображається у друкованих та PDF-виводах.

---

## Без друку

Вміст усередині блоку, який не друкується, видно на екрані, але приховано під час друку або експорту в PDF. Використовуйте його для інтерактивних вбудовуваних елементів, відео та посилань редактора, які не мають значення на друкованому аркуші.

### Знижка зі смаком малини

📖 [Специфікація RFM — Без друку](http://digital-docs.rpf-internal.org/docs/technology/codebases-and-products/raspberry-flavoured-markdown/specs/raspberry-flavoured-markdown-draft-spec#no-print)

```markdown
> [!NOPRINT]
>
> [Відкрийте стартовий проект метеостанції в редакторі](https://editor.raspberrypi.org/uk-UA/projects/weather-station)
```

> [Відкрийте стартовий проєкт метеостанції в редакторі](https://editor.raspberrypi.org/uk-UA/projects/weather-station)

### Спадщина Крамдаун РПФ

📖 [Специфікація Kramdown — Без друку](http://digital-docs.rpf-internal.org/docs/technology/codebases-and-products/raspberry-flavoured-markdown/specs/kramdown_rpf-legacy-spec#no-print)

```markdown
--- без друку ---

[Відкрийте стартовий проект метеостанції в редакторі](https://editor.raspberrypi.org/uk-UA/projects/weather-station)

--- /без друку ---
```

[Відкрийте стартовий проєкт метеостанції в редакторі](https://editor.raspberrypi.org/uk-UA/projects/weather-station)

---

## Тільки для друку

Вміст усередині блоку, доступного лише для друку, видно лише під час друку або експорту в PDF. Використовуйте його для створення статичних альтернатив інтерактивному контенту, наприклад, знімка екрана замість вбудованого редактора чи відео.

### Знижка зі смаком малини

📖 [Специфікація RFM — Тільки для друку](http://digital-docs.rpf-internal.org/docs/technology/codebases-and-products/raspberry-flavoured-markdown/specs/raspberry-flavoured-markdown-draft-spec#print-only)

```markdown
> [!ТІЛЬКИ ДЛЯ ДРУКУ]
>
> ![Знімок екрана завершеного проекту метеостанції](images/sense-hat-emulator.png)
```

> ![Знімок екрана завершеного проекту метеостанції](images/sense-hat-emulator.png)

### Спадщина Крамдаун РПФ

📖 [Специфікація Kramdown — Тільки друк](http://digital-docs.rpf-internal.org/docs/technology/codebases-and-products/raspberry-flavoured-markdown/specs/kramdown_rpf-legacy-spec#print-only)

```markdown
--- лише для друку ---

![Знімок екрана завершеного проекту метеостанції](images/sense-hat-emulator.png)

--- /лише для друку ---
```

![Знімок екрана завершеного проекту метеостанції](images/sense-hat-emulator.png)

---

## Розрив сторінки

Розрив сторінки примусово створює нову сторінку під час друку або експорту в PDF-аркуш. Розмістіть його між розділами, щоб забезпечити чисте макетування сторінки під час друку.

### Знижка зі смаком малини

📖 [Специфікація RFM — Розрив сторінки](http://digital-docs.rpf-internal.org/docs/technology/codebases-and-products/raspberry-flavoured-markdown/specs/raspberry-flavoured-markdown-draft-spec#page-break)

```markdown
Цей вміст відображається перед розривом сторінки.

{.page-break}

Цей вміст відображається на новій сторінці після розриву.
```

Цей вміст відображається перед розривом сторінки.

{.page-break}

Цей контент з’явиться на новій сторінці після перерви.

### Спадщина Крамдаун РПФ

📖 [Специфікація Kramdown — Нова сторінка](http://digital-docs.rpf-internal.org/docs/technology/codebases-and-products/raspberry-flavoured-markdown/specs/kramdown_rpf-legacy-spec#new-page)

```markdown
Вміст першої сторінки.


Вміст другої сторінки.
```

Вміст першої сторінки.

Зміст другої сторінки.
