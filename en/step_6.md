## Collapsible

Collapsible blocks (also called ingredient panels) contain supplementary content such as installation instructions or reference material. Learners can expand or collapse the panel as needed.

---

### Raspberry Flavoured Markdown

📖 [RFM spec — Collapsible](http://digital-docs.rpf-internal.org/docs/technology/codebases-and-products/raspberry-flavoured-markdown/specs/raspberry-flavoured-markdown-draft-spec#collapsible)

```markdown
> [!ACCORDION] How to open Thonny 
>
> Click the **Raspberry Pi menu**, then **Programming**, then **Thonny Python IDE**.
```

> [!ACCORDION] How to open Thonny 
>
> Click the **Raspberry Pi menu**, then **Programming**, then **Thonny Python IDE**.

---

### Kramdown RPF legacy

The legacy `collapse` block requires a YAML front matter section with a `title` field. The body is parsed as Markdown.

**Simple collapse**

📖 [Kramdown spec — Collapse](http://digital-docs.rpf-internal.org/docs/technology/codebases-and-products/raspberry-flavoured-markdown/specs/kramdown_rpf-legacy-spec#collapse)

```markdown
--- collapse ---
---
title: How to open Thonny
---

Click the **Raspberry Pi menu**, then **Programming**, then **Thonny Python IDE**.

--- /collapse ---
```

--- collapse ---
---
title: How to open Thonny
---

Click the **Raspberry Pi menu**, then **Programming**, then **Thonny Python IDE**.

--- /collapse ---

**Inside a list item**

📖 [Kramdown spec — Collapse (inside a list item)](http://digital-docs.rpf-internal.org/docs/technology/codebases-and-products/raspberry-flavoured-markdown/specs/kramdown_rpf-legacy-spec#inside-a-list-item)

````markdown
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
````

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
