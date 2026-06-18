## Підказки

Використовуйте підказки, щоб надавати покрокову допомогу учням, які зазнають труднощів. Підказки відображаються у каруселі свайперів, щоб учні могли відкривати їх по одній.

---

### Знижка зі смаком малини

Один блок `[!HINT]` відображається на повній панелі свайпера з маркованими сторінками.

📖 [Специфікація RFM — Підказка (одинарна)](http://digital-docs.rpf-internal.org/docs/technology/codebases-and-products/raspberry-flavoured-markdown/specs/raspberry-flavoured-markdown-draft-spec#hint-single)

```markdown
> [!ПІДКАЗКА]
>
> Перед запуском коду переконайтеся, що ваш Sense HAT надійно підключений до всіх 40 контактів GPIO.
```

> Перед запуском коду перевірте, чи ваш Sense HAT надійно підключений до всіх 40 контактів GPIO.

Коли у вихідному коді з'являються два або більше послідовних блоків `[!HINT]`, вони групуються в одну панель свайпера.

📖 [Специфікація RFM — Підказки (згруповані)](http://digital-docs.rpf-internal.org/docs/technology/codebases-and-products/raspberry-flavoured-markdown/specs/raspberry-flavoured-markdown-draft-spec#hints-grouped)

```markdown
> [!ПІДКАЗКА]
>
> Підказка 1: Імпортуйте `SenseHat` з бібліотеки `sense_hat`.

> [!ПІДКАЗКА]
>
> Підказка 2: Створіть об'єкт `SenseHat`: `sense = SenseHat()`

> [!ПІДКАЗКА]
>
> Підказка 3: Викличте `sense.get_temperature()`, щоб зчитати поточну температуру.
```

> Підказка 1: Імпортуйте `SenseHat` з бібліотеки `sense_hat`.

> Підказка 2: Створіть об'єкт `SenseHat`: `sense = SenseHat()`

> Підказка 3: Викличте `sense.get_temperature()`, щоб зчитати поточну температуру.

---

### Спадщина Крамдаун РПФ

У застарілому синтаксисі окремий блок `hint` відображається як окремий елемент swiper slide без навколишньої панелі-обгортки.

📖 [Специфікація Kramdown — Підказка (окрема)](http://digital-docs.rpf-internal.org/docs/technology/codebases-and-products/raspberry-flavoured-markdown/specs/kramdown_rpf-legacy-spec#hint)

```markdown

Окремий блок `hint` відображається як окремий елемент слайдера.

```

Окремий блок `hint` відображатиметься як окремий елемент слайдера.

Блок «підказок» обгортає один або декілька блоків «підказок» на повній панелі свайпера з кнопками навігації та крапками нумерації сторінок.

📖 [Специфікація Крамдауна — Підказки](http://digital-docs.rpf-internal.org/docs/technology/codebases-and-products/raspberry-flavoured-markdown/specs/kramdown_rpf-legacy-spec#hints)

```markdown

Підказка 1: Імпортуйте `SenseHat` з бібліотеки `sense_hat`.


Підказка 2: Створіть екземпляр `SenseHat`: `sense = SenseHat()`


Підказка 3: Використовуйте `sense.get_temperature()` для зчитування значення датчика температури.

```

Підказка 1: Імпортуйте `SenseHat` з бібліотеки `sense_hat`.

Підказка 2: Створіть екземпляр `SenseHat`: `sense = SenseHat()`

Підказка 3: Використовуйте `sense.get_temperature()` для зчитування значення датчика температури.

