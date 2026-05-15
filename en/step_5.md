## Code block

Code blocks display syntax-highlighted source code with optional filename labels, line numbers, and line highlights.

---

### Raspberry Flavoured Markdown

The RFM codeblock uses a standard fenced code block with metadata attributes on the opening fence line.

📖 [RFM spec — Codeblock](http://digital-docs.rpf-internal.org/docs/technology/codebases-and-products/raspberry-flavoured-markdown/specs/raspberry-flavoured-markdown-draft-spec#codeblock)

````markdown
```python filename="weather.py" line_numbers="true" line_number_start="3" line_highlights="3,5-6"
while True:
    temperature = sense.get_temperature()
    humidity = sense.get_humidity()
    sense.show_message(str(round(temperature, 1)))
    sleep(2)
```
````

```python filename="weather.py" line_numbers="true" line_number_start="3" line_highlights="3,5-6"
while True:
    temperature = sense.get_temperature()
    humidity = sense.get_humidity()
    sense.show_message(str(round(temperature, 1)))
    sleep(2)
```

---

### Kramdown RPF legacy

The legacy syntax uses a `--- code ---` block with a YAML front matter section for configuration.

**Language only**

📖 [Kramdown spec — Code block](http://digital-docs.rpf-internal.org/docs/technology/codebases-and-products/raspberry-flavoured-markdown/specs/kramdown_rpf-legacy-spec#code-block)

```markdown
--- code ---
---
filename: weather.py
language: python
line_numbers: true
line_number_start: 3
line_highlights: 3, 5-6
---
while True:
    temperature = sense.get_temperature()
    humidity = sense.get_humidity()
    sense.show_message(str(round(temperature, 1)))
    sleep(2)
--- /code ---
```

--- code ---
---
filename: weather.py
language: python
line_numbers: true
line_number_start: 3
line_highlights: 3, 5-6
---
while True:
    temperature = sense.get_temperature()
    humidity = sense.get_humidity()
    sense.show_message(str(round(temperature, 1)))
    sleep(2)
--- /code ---
