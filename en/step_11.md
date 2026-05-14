## Nested blocks

Blocks can be nested — for example, a `[!TASK]` can contain one or more `[!HINT]` blocks. Consecutive `[!HINT]` blocks nested inside a task are grouped into a single hints panel.

---

### Raspberry Flavoured Markdown

📖 [RFM spec — Nested blocks](http://localhost:3000/docs/technology/codebases-and-products/raspberry-flavoured-markdown/specs/raspberry-flavoured-markdown-draft-spec#nested-blocks)

> [!TASK]
>
> Read the temperature from the Sense HAT and display it on the LED matrix.
>
> > [!HINT]
> >
> > Hint 1: Use `sense.get_temperature()` to read the temperature value.
>
> > [!HINT]
> >
> > Hint 2: Round the result with `round(temperature, 1)` before displaying it.
