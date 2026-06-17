## Hints

Use hints to provide optional, step-by-step help for learners who get stuck. Hints are displayed in a swiper carousel so learners can reveal them one at a time.

---

### Raspberry Flavoured Markdown

A single `[!HINT]` block renders in a full swiper panel with pagination bullets.

📖 [RFM spec — Hint (single)](http://digital-docs.rpf-internal.org/docs/technology/codebases-and-products/raspberry-flavoured-markdown/specs/raspberry-flavoured-markdown-draft-spec#hint-single)

```markdown
> [!HINT]
>
> Check that your Sense HAT is firmly connected to all 40 GPIO pins before running your code.
```

> [!HINT]
>
> Check that your Sense HAT is firmly connected to all 40 GPIO pins before running your code.

When two or more consecutive `[!HINT]` blocks appear in the source, they are grouped into a single swiper panel.

📖 [RFM spec — Hints (grouped)](http://digital-docs.rpf-internal.org/docs/technology/codebases-and-products/raspberry-flavoured-markdown/specs/raspberry-flavoured-markdown-draft-spec#hints-grouped)

```markdown
> [!HINT]
>
> Hint 1: Import `SenseHat` from the `sense_hat` library.

> [!HINT]
>
> Hint 2: Create a `SenseHat` object: `sense = SenseHat()`

> [!HINT]
>
> Hint 3: Call `sense.get_temperature()` to read the current temperature.
```

> [!HINT]
>
> Hint 1: Import `SenseHat` from the `sense_hat` library.

> [!HINT]
>
> Hint 2: Create a `SenseHat` object: `sense = SenseHat()`

> [!HINT]
>
> Hint 3: Call `sense.get_temperature()` to read the current temperature.

---

### Kramdown RPF legacy

In the legacy syntax a standalone `hint` block renders as a single swiper slide element without the surrounding panel wrapper.

📖 [Kramdown spec — Hint (standalone)](http://digital-docs.rpf-internal.org/docs/technology/codebases-and-products/raspberry-flavoured-markdown/specs/kramdown_rpf-legacy-spec#hint)

```markdown
--- hint ---

A standalone `hint` block renders as a single swiper slide element.

--- /hint ---
```

--- hint ---

A standalone `hint` block renders as a single swiper slide element.

--- /hint ---

A `hints` block wraps one or more `hint` blocks in the full swiper panel with navigation buttons and pagination dots.

📖 [Kramdown spec — Hints](http://digital-docs.rpf-internal.org/docs/technology/codebases-and-products/raspberry-flavoured-markdown/specs/kramdown_rpf-legacy-spec#hints)

```markdown
--- hints ---
--- hint ---

Hint 1: Import `SenseHat` from the `sense_hat` library.

--- /hint ---
--- hint ---

Hint 2: Create a `SenseHat` instance: `sense = SenseHat()`

--- /hint ---
--- hint ---

Hint 3: Use `sense.get_temperature()` to read the temperature sensor value.

--- /hint ---
--- /hints ---
```

--- hints ---
--- hint ---

Hint 1: Import `SenseHat` from the `sense_hat` library.

--- /hint ---
--- hint ---

Hint 2: Create a `SenseHat` instance: `sense = SenseHat()`

--- /hint ---
--- hint ---

Hint 3: Use `sense.get_temperature()` to read the temperature sensor value.

--- /hint ---
--- /hints ---
