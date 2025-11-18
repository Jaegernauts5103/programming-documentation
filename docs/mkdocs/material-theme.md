# Customizing the Material Theme

This page explains how to customize the **Material for MKDocs** theme used in MECH & Cheese documentation. By following these guidelines, you can adjust the appearance, layout, and features to match our team branding and improve usability.

---

## 1. Changing the Theme Colors

Material allows you to define **primary** and **accent colors** in `mkdocs.yml`:

```yml
theme:
  name: material
  palette:
    primary: 'deep orange'
    accent: 'orange'
```

* You can use [Material color names](https://squidfunk.github.io/mkdocs-material/setup/changing-the-colors/) or hex codes.
* Recommended for MECH & Cheese: **primary: #4051B5** (team color), **accent: #4051B5** (can be changed).

---

## 2. Adding a Logo

You can display the team logo in the header:

```yml
theme:
  name: material
  logo: images/mech_cheese_logo.png
```

* Place the image in your `docs/images/` folder
* Recommended size: **~40-80px height** for header

---

## 3 Configuring the Navigation

The **sidebar** and **top navigation** can be customized in `mkdocs.yml`:

```yml
nav:
  - Overview: index.md
  - Getting Started: getting-started.md
  - Chassis:
      - Overview: chassis/overview.md
      - Wiring: chassis/wiring.md
```

Tips:
* Use folders for topics to keep the sidebar organized
* Use descriptive names to help new members quickly find information

## 4. Enabling Search

Material includes a built-in search bar. To enable:

```yml
theme:
  name: material
  features:
    - search.highlight
    - search.suggest
```

* `search.highlight` highlights matching terms
* `search.suggest` provides suggestions while typing

---

## 5. Enabling Code Copy Buttons

Make all fenced code blocks easier to copy:

```yml
theme:
  name: material
  features:
    - content.code.copy
```

* Adds a small copy icon to the top-right of each code block
* Works automatically on fenced code blocks with language specified:

```bash
git clone https://github.com/Jaegernauts5103/programming-documentation.git
```

---

## 6. Using Tabs and Collapsible Sections

Material supports advanced formatting like **tabs** and **collapsible sections** for better organization:

**Tabs Example:**

```md
=== "Python"

    ```python
    print("Hello, world!")
    ```

=== "Java"

    ```java
    System.out.println("Hello, world!");
    ```

```

**Collapsible Section Example:**

```md
??? note "Important Note"
    Always disconnect power before working on wiring.
```

---

## 7. Custom Fonts and Icons

You can customize fonts and icons in `mkdocs.yml` using `extra`:

```yml
extra:
  font:
    text: "Roboto"
    code: "Fira Code"
```

* `text`: font for body text
* `code`: font for code blocks
* Icons can be adding using Material icon syntax in Markdown

---

## 8. Summary

Customizing Material for MKDocs allows MECH & Cheese documentation to:

* Match team branding
* Improve navigation and readability
* Enhance usability for new members
* Include professional styling with minimal effort

> 💡 Tip: Always preview changes locally using `mkdocs serve` before committing to GitHub.