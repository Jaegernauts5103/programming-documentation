# Project Structure & Best Practices

This page explains the recommended **project structure** for MECH & Cheese’s MKDocs documentation and provides best practices for writing and organizing content. Following these guidelines will make your documentation professional, maintainable, and easy for new members to contribute to.

---

## 1. Recommended Folder Structure

Organizing your files consistently prevents confusion as the documentation grows.

```md
programming-documentation/
├─ mkdocs.yml
├─ docs/
│ ├─ index.md # Overview page
│ ├─ getting-started.md
│ ├─ chassis/
│ │ ├─ overview.md
│ │ ├─ wiring.md
│ │ └─ maintenance.md
│ ├─ programming/
│ │ ├─ overview.md
│ │ ├─ subsystems.md
│ │ └─ commands.md
│ ├─ sensors/
│ │ └─ overview.md
│ └─ reference/
│ └─ glossary.md
```
---

**Notes:**

- Each main topic gets its **own folder** inside of the `docs` folder (`chassis/`, `programming/`, `sensors/`)
- Each folder can have multiple Markdown pages for specific topics
- `index.md` serves as the landing page for the documentation
- Keep file names **lowercase and hyphenated** for consistency

---

## 2. Navigation & Sidebar

The sidebar is defined in `mkdocs.yml`. Example:

```yaml
nav:
  - Overview: index.md
  - Getting Started: getting-started.md
  - Chassis:
      - Overview: chassis/overview.md
      - Wiring: chassis/wiring.md
      - Maintenance: chassis/maintenance.md
  - Programming:
      - Overview: programming/overview.md
      - Subsystems: programming/subsystems.md
      - Commands: programming/commands.md
  - Sensors:
      - Overview: sensors/overview.md
  - Reference:
      - Glossary: reference/glossary.md
```

### Best Practices

* Order pages logically, top-level topics first
* Use folders for subtopics rather than long page names
* Update the sidebar whenever new pages are added

### Markdown File Naming

* Use lowercase letters
* Use hyphens to separate words (`robot-setup.md`)
* Keep names short but descriptive

---

## 4. Writing Guidelines

* Use headings consistently (# for main titles, ## for sections, ### for sub-sections)
* Use fenced code blocks for commands:

```bash
git clone https://github.com/Jaegernauts5103/programming-documentation.git
```

* Use bold for important terms (**PID loop**)
* Use links to other pages:

```md
[Chassis Overview](chassis/overview.md)
```

* Use lists for instructions:

```md
1. Install dependencies
2. Clone the repository
3. Run mkdocs serve
```

* Add images for diagrams, wiring, and examples:

```md
![Motor Wiring Diagram](images/motor-wiring.png)
```

---

## 5. Best Practices for Collaboration

* Always preview locally with mkdocs serve before committing
* Pull changes regularly: git pull origin main
* Write clear commit messages for documentation updates
* Use the established folder structure when adding new content

---

## 6. Summary

Following this structure and these practices ensures that:

* Documentation stays organized and navigable
* New members can quickly find relevant information
* Updates are easy to track and merge
* Your MKDocs site remains professional and readable

> Tip: Before adding a new page, ask yourself:

* Does it fit under an existing folder, or does it need a new topic folder?
* Is the page name clear and descriptive?
* Will it be easy to link from the sidebar or other pages?