## Code block

Code blocks display syntax-highlighted source code with optional filename labels, line numbers, and line highlights.

---

### Raspberry Flavoured Markdown

The RFM codeblock uses a standard fenced code block with metadata attributes on the opening fence line.

📖 [RFM spec — Codeblock](http://localhost:3000/docs/technology/codebases-and-products/raspberry-flavoured-markdown/specs/raspberry-flavoured-markdown-draft-spec#codeblock)

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

📖 [Kramdown spec — Code block](http://localhost:3000/docs/technology/codebases-and-products/raspberry-flavoured-markdown/specs/kramdown_rpf-legacy-spec#code-block)

--- code ---
---
language: python
---
print("Hello, World!")
--- /code ---

**With filename**

--- code ---
---
language: python
filename: hello.py
---
print("Hello, World!")
--- /code ---

**With line numbers**

--- code ---
---
language: python
line_numbers: true
---
print("Hello, World!")
--- /code ---

**With line highlights**

--- code ---
---
language: python
line_highlights: 1
---
print("Hello, World!")
--- /code ---

**With all features**

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

**Plain fenced code block**

```python
while True:
    temperature = sense.get_temperature()
    sleep(2)
```

**With line numbers disabled**

--- code ---
---
language: python
line_numbers: false
---
while True:
    temperature = sense.get_temperature()
    sleep(2)
--- /code ---
