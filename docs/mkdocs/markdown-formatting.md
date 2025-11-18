# Markdown Formatting & Best Practices

This page provides guidelines and examples for writing clean, consistent Markdown documentation for MECH & Cheese. Following these practices ensures readability, maintainability, and a professional appearance on your MKDocs site.

Each guideline includes the recommended code along with a preview of how it will appear on the site, when applicable.

---

## 1. Headings

Use headings to organize content hierarchically:

```markdown
# Main Title (H1)
## Section Title (H2)
### Subsection Title (H3)
#### Optional Sub-subsection (H4)
```

* Only one # per page for the main title.
* Use headings consistently to structure content clearly.

---

## 2. Text Formatting

* Bold important terms: **PID Loop** → PID Loop `**this bolds text!**`
* Italicize emphasis: *important note* → important note `*this italicizes text!*`
* Combine bold and italics: ***very important*** → very important `***this bolds and italicizes text!***`

---

## 3. Lists

**Unordered Lists**

```md
* First item
* Second item
  * Sub-item
* Third item
```

* First item
* Second item
  * Sub-item
* Third item

**Ordered Lists**

```md
1. Step one
2. Step two
   1. Sub-step
3. Step three
```
1. Step one
2. Step two
   1. Sub-step
3. Step three

---

## 4. Links

**Internal Links (within the documentation)**

```md
[Chassis Overview](chassis/overview.md)
```

**External Links**

```md
[MECH & Cheese GitHub](https://github.com/Jaegernauts5103/programming-documentation)
```

**Linking to Headings**

```md
[Motor Wiring](chassis/wiring.md#wiring-the-motors)
```

---

## 5. Code Blocks

**Inline Code**

Use backticks for inline code: ``Use `git clone` to copy the repo``

**Fenced Code Blocks**

````md
```bash
This is a fenced code block!
It can span as many lines as I want.

It can have gaps between lines.
It can also have no gap between lines
```
````

* Always use fenced code blocks with triple backticks.
* Include the language (bash, python, etc.) for syntax highlighting.
* With Material theme, a copy button can appear automatically on fenced code blocks.

---

## 6. Tables

```md
| Component       | Description           | Notes               |
|-----------------|-------------------|-------------------|
| Neo Motor       | Drive motor        | 400 RPM max       |
| Encoder         | Measures position  | Absolute, Rev     |
```

| Component       | Description           | Notes               |
|-----------------|-------------------|-------------------|
| Neo Motor       | Drive motor        | 400 RPM max       |
| Encoder         | Measures position  | Absolute, Rev     |

---

## 7. Images

* Place images in an images/ folder.
* Link using relative paths:

```md
![Motor Wiring Diagram](images/motor-wiring.png)
```

* Add descriptive alt text for clarity.

---

## 8. Blockquotes

Use for notes, warnings, or tips

```md
> ⚠️ Always disconnect power before working on wiring.
>
> Tip: Use a consistent color scheme for diagrams.
```

> This is a blockquote.
>
> It can span multiple lines.

---

## 9. Tips for Clean Documentation

* Keep sentences short and clear
* Break large sections into multiple pages if needed
* Preview regularly with mkdocs serve
* Use consistent terminology for subsystems, commands, and hardware
* Update links whenever pages are moved or renamed

---

## 10. Summary

* Following these Markdown formatting rules ensures that MECH & Cheese documentation is:
* Professional and readable
* Easy to navigate and maintain
* Ready for new members to contribute quickly
* Fully compatible with MKDocs and Material theme features, including code copy buttons and syntax highlighting