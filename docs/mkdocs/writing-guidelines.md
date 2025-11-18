# Writing Guidelines & Documentation Workflow

This page provides best practices for writing and maintaining MECH & Cheese documentation. Following these guidelines ensures that all team members can contribute efficiently, and that documentation remains consistent and professional over time.

---

## 1. General Writing Guidelines

- **Be clear and concise**: Use short sentences and simple language.
- **Use consistent terminology**: Refer to subsystems, commands, and hardware using agreed-upon names.
- **Use proper Markdown formatting**: Headings, lists, code blocks, and links should follow the standards outlined in the Markdown

Formatting page.

- **Add examples when helpful**: Show code snippets, wiring diagrams, or screenshots to illustrate instructions.  
- **Use relative links**: Always link to other pages or images using relative paths to avoid broken links.  

---

## 2. Page Organization

- Start with a **main heading** (`#`) for the page title.  
- Break content into **logical sections** using `##` or `###` headings.  
- Use lists, tables, and code blocks to make content easy to scan.  
- Include a **summary or key points** section at the end of longer pages.  

---

## 3. Workflow for Editing Documentation

### 1. **Preview Locally**  

   - Run `mkdocs serve` to preview changes before committing.  
   - Make sure formatting, links, and code blocks render correctly.

### 2. **Create a Branch (Optional but Recommended)**  

```bash
git checkout -b my-feature-branch
```

* Useful if multiple people are working on the documentation simultaneously

### 3. **Make Your Changes**

* Add or edit Markdown files in the appropriate folder
* Follow folder structure and naming conventions

### 4. **Commit Changes with Clear Messages**

```bash
git add .
git commit -m "Add wiring instructions for drive motors"
```

### 5. **Pull Latest Changes Before Pushing**

```bash
git pull origin main
```

### 6. **Push Changes to GitHub**

```bash
git push origin my-feature-branch
```

### 7. **Merge or Create Pull Requests**

* Use GitHub to merge your branch into `main`
* Review by another team member if possible to catch errors

---

## 4. Collaboration Best Practices

* Communicate with your team about which pages you’re editing.
* Avoid editing the same file simultaneously without coordination.
* Regularly pull changes from the main branch to avoid merge conflicts.
* Maintain consistent formatting across all pages (headings, lists, code blocks).

---

## 5. Updating Existing Pages

* Check the page for **outdated** information before making edits
* Preserve existing examples and formatting where possible
* Add a "**last updated**" note at the top or bottom if necessary:

```md
*Last updated: November 2025*
```

---

## 6. Summary

Following these writing guidelines and workflow steps ensures that MECH & Cheese documentation is:

* Professional and consistent
* Easy for new members to read and understand
* Easy to maintain and update over multiple seasons
* Collaborative, minimizing conflicts between team members

> 💡 Tip: Always preview your changes locally with mkdocs serve and check links and code blocks before pushing to GitHub.