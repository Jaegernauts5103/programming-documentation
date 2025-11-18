# FAQ & Troubleshooting

This page provides solutions to common issues encountered when using MKDocs, Material for MKDocs, or collaborating on MECH & Cheese documentation. It is intended to help new members resolve problems quickly without needing to ask for help.

---

## 1. Auto-Reload Not Working (`mkdocs serve`)

**Issue:** Changes do not appear automatically in the browser when editing Markdown files.  

**Solution:**
1. Stop the server by pressing **Ctrl + C** in PowerShell.  
2. Restart the server:

```bash
mkdocs serve
```

> 💡 Tip: Always use PowerShell instead of Command Prompt for better compatibility.

---

## 2. Broken Links or Images

**Issue:** Links to other pages or images do not work.

**Common Causes & Solutions:**

* Relative paths are incorrect
    * Check the path to the target file or image. For example, if an image is in `docs/images/`:

```md
~[Diagram](images/example.png)
```

* **File or folder renamged but links not updated**
    * Update all affected links in your Markdown files
* **Spaces or special characters in filenames**
    * Use lowercase letters and hgyphens (`motor-wiring.png`) instead of spaces

---

## 3. Git Merge Conflicts

**Issue:** Conflicts occur when multiple members edit the same file simultaneously

**Solution:**

**1.** Pull the latest changes:

```bash
git pull origin main
```

**2.** Resolve conflicts manually by editing the affected files.
**3.** Mark conflicts as resolved

```bash
git add <file>
git commit -m "Resolve merge conflict"
```

**4.** Push your changes back to GitHub

> 💡 Tip: Coordinate with teammates to avoid editing the same files at the same time.

---

## 4. Python or pip Issues

**Issue:** MKDocs or Material fails to install

**Solutions:**

* Make sure **Python 3.8 or later** is installed:

```bash
python --version
```

* **Ensure pip is installed and up-to-date:**

```bash
python -m ensurepip --upgrade
python -m pip install --upgrade pip
```

* Reinstall MKDocs and Material

```bash
pip install --upgrade mkdocs mkdocs-material
```

---

## 5. MKDocs Version Issues

**Issue:** Commands fail because the MKDocs version is outdated

**Solution:** Check the version:

```bash
mkdocs --version
```

Update if necessary:

```bash
pip install --upgrade mkdocs
pip install --upgrade mkdocs-material
```

---

## 6. Fenced Code Blocks Not Rendering Properly

**Issue:** Code blocks are not displayed correctly on the site

**Solutions:**

* Ensure you are using **triple backticks** (```) to fence the code block
* Specify the language for syntax highlighting:

````bash
```python
print("Hello, MECH & Cheese)
```
````

- For nested code blocks, use **more backticks for the outer block than the inner block**.

---

## 7. Preview Issues

**Issue:** The local preview does not reflect changes.  

**Solutions:**

1. Stop and restart the server (`Ctrl + C` → `mkdocs serve`).  
2. Clear the browser cache or use a private/incognito window.  
3. Make sure you are editing the correct `.md` file in the project folder.

---

## 8. Getting Help

If none of the above solutions work:  
- Check the [MKDocs Documentation](https://www.mkdocs.org/)  
- Check the [Material for MKDocs Documentation](https://squidfunk.github.io/mkdocs-material/)  
- Ask a MECH & Cheese mentor or team member for guidance.  

---

> 💡 Tip: Regularly preview, test links, and coordinate changes with teammates to avoid most common issues.
