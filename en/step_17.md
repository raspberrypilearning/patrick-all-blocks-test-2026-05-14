## Quiz and knowledge quiz question

The `quiz` block renders a simple non-marking radio poll. The `question` block renders a self-marking quiz question with a correct answer, optional per-choice feedback, and a customisable legend.

---

### Quiz

A `quiz` block is a simple radio-button poll with no correct answer. The question is defined in YAML front matter and choices use `( )` notation.

📖 [Kramdown spec — Quiz](http://localhost:3000/docs/technology/codebases-and-products/raspberry-flavoured-markdown/specs/kramdown_rpf-legacy-spec#quiz)

--- quiz ---
---
question: How are you feeling about this project so far?
---

- ( ) Ready to code!
- ( ) Still warming up
- ( ) A little confused — but curious

--- /quiz ---

---

### Knowledge quiz question — simple

A `question` block is a self-marking question. Choices use `( )` for wrong answers and `(x)` for the correct answer.

📖 [Kramdown spec — Knowledge quiz question](http://localhost:3000/docs/technology/codebases-and-products/raspberry-flavoured-markdown/specs/kramdown_rpf-legacy-spec#knowledge-quiz-question)

--- question ---

What does `sense.get_temperature()` return?

--- choices ---

- ( ) A string
- (x) A float
- ( ) An integer

--- /choices ---

--- /question ---

---

### Knowledge quiz question — with legend front matter

The fieldset legend can be overridden with a YAML front matter section inside the `question` block.

📖 [Kramdown spec — Knowledge quiz question (with legend)](http://localhost:3000/docs/technology/codebases-and-products/raspberry-flavoured-markdown/specs/kramdown_rpf-legacy-spec#with-legend-front-matter)

--- question ---

---
legend: Question 1 of 3
---

What temperature scale does `sense.get_temperature()` use?

--- choices ---

- (x) Celsius
- ( ) Fahrenheit
- ( ) Kelvin

--- /choices ---

--- /question ---

---

### Knowledge quiz question — with per-choice feedback

Individual `feedback` blocks attached to incorrect choices explain why they are wrong.

📖 [Kramdown spec — Knowledge quiz question (with per-choice feedback)](http://localhost:3000/docs/technology/codebases-and-products/raspberry-flavoured-markdown/specs/kramdown_rpf-legacy-spec#with-per-choice-feedback)

--- question ---

Which Raspberry Pi GPIO pin mode should you use to turn an LED on and off?

--- choices ---

- (x) Output

- ( ) Input

  --- feedback ---
  Input mode reads a signal — it cannot drive a component like an LED.
  --- /feedback ---

- ( ) PWM

  --- feedback ---
  PWM (pulse-width modulation) controls brightness, not simple on/off switching.
  --- /feedback ---

--- /choices ---

--- /question ---

---

### Knowledge quiz question — with single (global) feedback

A `feedback` block placed at the top of a `choices` block shows a hint for all wrong answers.

📖 [Kramdown spec — Knowledge quiz question (with single feedback)](http://localhost:3000/docs/technology/codebases-and-products/raspberry-flavoured-markdown/specs/kramdown_rpf-legacy-spec#with-single-feedback)

--- question ---

What food will the bug reach when these instructions are followed?

![A bug in a crossword-like maze with various bits of food scattered around](images/q2.svg)

1. Forward
2. Forward
3. Forward
4. Turn left
5. Forward
6. Forward
7. Turn right
8. Forward

--- choices ---

--- feedback ---
Follow the instructions one at a time. Which food item does the bug reach?
--- /feedback ---

- (x) Apple
- ( ) Banana
- ( ) Orange
- ( ) Doughnut

--- /choices ---

--- /question ---

---

### Knowledge quiz question — with blocks in feedback

Feedback blocks can contain fenced code blocks, including `blocks3` for Scratch block diagrams.

📖 [Kramdown spec — Knowledge quiz question (with blocks in feedback)](http://localhost:3000/docs/technology/codebases-and-products/raspberry-flavoured-markdown/specs/kramdown_rpf-legacy-spec#with-blocks-in-feedback)

--- question ---

A cat sprite in Scratch has the following code attached to it:

![A cat with three Scratch blocks](images/q1.svg)

How would you make the cat sprite change size?

--- choices ---

- ( ) Press the space key

  --- feedback ---
  What code is attached to the
  ```blocks3
  when [space v] key pressed
  ```
  event block?
  --- /feedback ---

- ( ) Click the green flag

  --- feedback ---
  What code is attached to the
  ```blocks3
  when flag clicked
  ```
  event block?
  --- /feedback ---

- (x) Click on the cat sprite

--- /choices ---

--- /question ---
