## Вступ

Цей проєкт тестує всі користувацькі типи блоків Markdown як зі специфікації Raspberry Flavoured Markdown, так і зі застарілої специфікації Kramdown RPF. Кожен крок охоплює один тип блоку та показує приклади з обох специфікацій, де блок існує в обох специфікаціях.

Якщо блок існує в обох специфікаціях, приклад **Малинового смаку Markdown** показано першим, а потім приклад **Kramdown RPF legacy**. Вихідний код markdown для кожного прикладу відображається в блоці коду безпосередньо перед відрендереним виводом.

Дві специфікації, на які посилаються в цьому проєкті:

- [Малиновий смак Markdown — Чернетка специфікації](http://digital-docs.rpf-internal.org/docs/technology/codebases-and-products/raspberry-flavoured-markdown/specs/raspberry-flavoured-markdown-draft-spec) — сучасний синтаксис сповіщень на основі GFM (`> [!BLOCK]`), що використовується `rpf-markdown-core`
- [Kramdown RPF — Застаріла специфікація](http://digital-docs.rpf-internal.org/docs/technology/codebases-and-products/raspberry-flavoured-markdown/specs/kramdown_rpf-legacy-spec) — старіший синтаксис `--- block ---` / `--- /block ---`, що використовується `kramdown-rpf`

У прикладах як робочий зразок контенту використовується метеостанція Raspberry Pi Sense HAT.
