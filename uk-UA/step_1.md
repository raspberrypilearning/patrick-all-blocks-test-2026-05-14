## Introduction

This project tests all custom Markdown block types from both the Raspberry Flavoured Markdown spec and the Kramdown RPF legacy spec. Each step covers one block type and shows examples from both specifications where a block exists in both specs.

Where a block exists in both specs, the **Raspberry Flavoured Markdown** example is shown first, followed by the **Kramdown RPF legacy** example. The markdown source for each example is shown in a code block immediately before the rendered output.

The two specifications referenced throughout this project are:

- [Raspberry Flavoured Markdown — Draft Spec](http://digital-docs.rpf-internal.org/docs/technology/codebases-and-products/raspberry-flavoured-markdown/specs/raspberry-flavoured-markdown-draft-spec) — the modern GFM-based alert syntax (`> [!BLOCK]`), used by `rpf-markdown-core`
- [Kramdown RPF — Legacy Spec](http://digital-docs.rpf-internal.org/docs/technology/codebases-and-products/raspberry-flavoured-markdown/specs/kramdown_rpf-legacy-spec) — the older `--- block ---` / `--- /block ---` syntax, used by `kramdown-rpf`

The examples use a Raspberry Pi Sense HAT weather station as running sample content.
