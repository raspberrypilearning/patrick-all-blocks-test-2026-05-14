## Task

Task blocks wrap a discrete unit of work. They render with a checkbox that learners can tick when they complete the step. Tasks can contain code, hints, and collapsible panels.

---

### Raspberry Flavoured Markdown

📖 [RFM spec — Task](http://digital-docs.rpf-internal.org/docs/technology/codebases-and-products/raspberry-flavoured-markdown/specs/raspberry-flavoured-markdown-draft-spec#task)

```markdown
> [!TASK]
>
> Complete this step.
```

> [!TASK]
>
> Complete this step.

---

### Kramdown RPF legacy

A basic task containing code and prose.

📖 [Kramdown spec — Task](http://digital-docs.rpf-internal.org/docs/technology/codebases-and-products/raspberry-flavoured-markdown/specs/kramdown_rpf-legacy-spec#task)

````markdown
--- task ---

Add the `global` keyword so the function can update the `temperature` variable:

```python
def update_display(event):
    global temperature
```

You can now read and write `temperature` from inside `update_display`.

--- /task ---
````

--- task ---

Add the `global` keyword so the function can update the `temperature` variable:

```python
def update_display(event):
    global temperature
```

You can now read and write `temperature` from inside `update_display`.

--- /task ---

#### With hints

Tasks can contain a `hints` block to give learners optional help without cluttering the main step.

📖 [Kramdown spec — Task (with hints)](http://digital-docs.rpf-internal.org/docs/technology/codebases-and-products/raspberry-flavoured-markdown/specs/kramdown_rpf-legacy-spec#with-hints)

```markdown
--- task ---

Read the current temperature and display it on the Sense HAT LED matrix.

--- hints ---
--- hint ---

Hint 1: Call `sense.get_temperature()` to read the temperature.

--- /hint ---
--- hint ---

Hint 2: Store the result: `temperature = sense.get_temperature()`

--- /hint ---
--- hint ---

Hint 3: Display it with `sense.show_message(str(round(temperature, 1)))`.

--- /hint ---
--- /hints ---

--- /task ---
```

--- task ---

Read the current temperature and display it on the Sense HAT LED matrix.

--- hints ---
--- hint ---

Hint 1: Call `sense.get_temperature()` to read the temperature.

--- /hint ---
--- hint ---

Hint 2: Store the result: `temperature = sense.get_temperature()`

--- /hint ---
--- hint ---

Hint 3: Display it with `sense.show_message(str(round(temperature, 1)))`.

--- /hint ---
--- /hints ---

--- /task ---

#### With collapsible ingredient

Tasks can also contain a `collapse` block to embed ingredient content inline.

📖 [Kramdown spec — Task (with ingredient)](http://digital-docs.rpf-internal.org/docs/technology/codebases-and-products/raspberry-flavoured-markdown/specs/kramdown_rpf-legacy-spec#with-ingredient)

````markdown
--- task ---

Set up your Raspberry Pi and install the required software.

--- collapse ---
---
title: How to install the Sense HAT library
---

Open a terminal and run:

```bash
pip install sense-hat
```

Reboot your Raspberry Pi after installation.

--- /collapse ---

--- /task ---
````

--- task ---

Set up your Raspberry Pi and install the required software.

--- collapse ---
---
title: How to install the Sense HAT library
---

Open a terminal and run:

```bash
pip install sense-hat
```

Reboot your Raspberry Pi after installation.

--- /collapse ---

--- /task ---
