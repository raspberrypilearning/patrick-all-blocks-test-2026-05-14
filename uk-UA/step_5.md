## Блок коду

Блоки коду відображають вихідний код із виділеним синтаксисом, а також додатковими мітками назв файлів, номерами рядків та виділенням рядків.

---

### Знижка зі смаком малини

Кодовий блок RFM використовує стандартний огороджений блок коду з атрибутами метаданих на початковій лінії огорожі.

📖 [Специфікація RFM — Блок коду](http://digital-docs.rpf-internal.org/docs/technology/codebases-and-products/raspberry-flavoured-markdown/specs/raspberry-flavoured-markdown-draft-spec#codeblock)

````markdown
```python filename="weather.py" line_numbers="true" line_number_start="3" line_highlights="3,5-6"
while True:
    температура = sense.get_temperature()
    вологість = sense.get_humidity()
    sense.show_message(str(round(температура, 1)))
    сліп(2)
```
````

```python filename="weather.py" line_numbers="true" line_number_start="3" line_highlights="3,5-6"
поки True:
    температура = sense.get_temperature()
    вологість = sense.get_humidity()
    sense.show_message(str(round(температура, 1)))
    сплячий режим(2)
```

---

### Спадщина Крамдаун РПФ

У застарілому синтаксисі для налаштування використовується блок `--- code ---` з розділом початкового коду YAML.

**Тільки мова**

📖 [Специфікація Kramdown — Блок коду](http://digital-docs.rpf-internal.org/docs/technology/codebases-and-products/raspberry-flavoured-markdown/specs/kramdown_rpf-legacy-spec#code-block)

```markdown
---
ім'я файлу: weather.py
мова: python
line_numbers: true
line_number_start: 3
line_highlights: 3, 5-6
---
while True:
    температура = sense.get_temperature()
    вологість = sense.get_humidity()
    sense.show_message(str(round(температура, 1)))
    sleep(2)
```

---

--- code ---
ім'я файлу: weather.py
мова: python
line_numbers: true
line_number_start: 3
line_highlights: 3, 5-6
------------------------------------------------------------

поки True:
температура = sense.get_temperature()
вологість = sense.get_humidity()
sense.show_message(str(round(температура, 1)))
сплячий режим(2)
--- /code ---
