## Microbit and Scratch code blocks

Fenced code blocks with specialist language identifiers render with matching CSS classes, which are picked up by interactive widgets in the page.

---

### Microbit code block

A fenced code block with the language identifier `microbit` renders with `class="language-microbit"`, which the BBC micro:bit simulator widget uses to display an interactive preview.

📖 [Kramdown spec — Microbit code block](http://localhost:3000/docs/technology/codebases-and-products/raspberry-flavoured-markdown/specs/kramdown_rpf-legacy-spec#microbit-code-block)

```microbit
from microbit import *

while True:
    display.show(Image.HEART)
    sleep(1000)
    display.clear()
    sleep(1000)
```

---

### Scratch code blocks

Fenced code blocks with the language `blocks3` (Scratch 3) or `blocks` (Scratch 2) render with the corresponding CSS class. The scratchblocks rendering library picks up these classes to draw visual Scratch block representations.

**Scratch 3 (`blocks3`)**

📖 [Kramdown spec — Scratch code blocks](http://localhost:3000/docs/technology/codebases-and-products/raspberry-flavoured-markdown/specs/kramdown_rpf-legacy-spec#scratch-code-blocks)

```blocks3
when flag clicked
repeat (10)
  move (10) steps
end
```

**Scratch 2 (`blocks`)**

```blocks
when flag clicked
repeat (10)
  move (10) steps
```
