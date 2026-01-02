# Sample Accessible EPUB

This repository contains a minimal, **born-accessible EPUB** example.
Designed for indie authors, publishers, and developers to reference **accessibility metadata, semantic structure, and alt text practices** in EPUB 3.3.

This sample was produced via **Monoline**, our preferred EPUB pipeline, to demonstrate proper accessibility compliance and clean structure.

---

## What's in this repo

```
sample-accessible-epub/
├── content.opf       # EPUB metadata, manifest, spine, accessibility info
├── nav.xhtml         # Navigation (TOC)
├── chapter1.xhtml    # Sample chapter 1
├── chapter2.xhtml    # Sample chapter 2
├── css/
│   └── style.css     # Minimal styling
└── images/
    └── sample.jpg    # Placeholder image with alt text
```

* Each XHTML file is structured semantically.
* `<h1>` for chapter titles, `<h2>` for sub-sections.
* Lists, paragraphs, and images include proper markup and alt attributes.
* `content.opf` includes **born-accessible metadata** (`schema:accessibilityFeature`, `schema:accessibilitySummary`).

---

## How to use

1. Clone this repository:

```bash
git clone https://github.com/YourUsername/sample-accessible-epub.git
cd sample-accessible-epub
```

2. Test locally using an EPUB reader (Calibre, Thorium, Adobe Digital Editions, etc.).

3. Optional: **Validate EPUB** using [EPUBCheck](https://github.com/w3c/epubcheck):

```bash
epubcheck sample.epub
```

> Zip the folder contents into `sample.epub` before running EPUBCheck.

4. Reference the structure and metadata when creating your own accessible EPUBs.

---

## Why it matters

* **EU Accessibility Act (EAA)** now requires all ebooks sold in the EU to meet accessibility standards.
* Older EPUBs without accessibility metadata or semantic markup may **fail compliance checks**.
* This sample provides a **baseline** for born-accessible ebooks.

---

## Credits: Monoline

This repository is a **Monoline-endorsed sample**, showing the accessibility workflow we apply across production pipelines: semantic markup, alt text, clean CSS, and proper EPUB metadata.

For more info: [Monoline](https://www.monoline.net)

---

## License

This sample is **CC0 / Public Domain**. Use it freely for testing, teaching, or reference.
