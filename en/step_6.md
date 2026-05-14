## Collapsible

Collapsible blocks (also called ingredient panels) contain supplementary content such as installation instructions or reference material. Learners can expand or collapse the panel as needed.

---

### Raspberry Flavoured Markdown

📖 [RFM spec — Collapsible](http://localhost:3000/docs/technology/codebases-and-products/raspberry-flavoured-markdown/specs/raspberry-flavoured-markdown-draft-spec#collapsible)

> [!ACCORDION] Downloading and installing the Raspberry Pi software
>
> Content here comes from the ingredient.

---

### Kramdown RPF legacy

The legacy `collapse` block requires a YAML front matter section with a `title` field. The body is parsed as Markdown.

**Simple collapse**

📖 [Kramdown spec — Collapse](http://localhost:3000/docs/technology/codebases-and-products/raspberry-flavoured-markdown/specs/kramdown_rpf-legacy-spec#collapse)

--- collapse ---
---
title: How to open Thonny
---

Click the **Raspberry Pi menu**, then **Programming**, then **Thonny Python IDE**.

--- /collapse ---

**With a code block in the body**

--- collapse ---
---
title: Starter code for weather.py
---

<div class="c-code-filename">
  weather.py
</div>
<pre dir="ltr" class="line-numbers" data-start="1"><code class="language-python" dir="ltr">
from sense_hat import SenseHat
from time import sleep

sense = SenseHat()

while True:
    temperature = sense.get_temperature()
    print(round(temperature, 1))
    sleep(2)
</code></pre>

--- /collapse ---

**Inside a list item**

1. Open Thonny on your Raspberry Pi.

    --- collapse ---
    ---
    title: Opening Thonny
    ---

    Click **Raspberry Pi menu > Programming > Thonny Python IDE**.

    --- /collapse ---

1. Create a new file and save it as **weather.py**.

1. Add your imports at the top of the file:

    ```python
    from sense_hat import SenseHat
    from time import sleep
    ```
