# Importing from GitHub

This page covers how **MECH & Cheese** members can import the team documentation from GitHub.  
If another FRC team wishes to use this documentation as a template, you are welcome to clone or fork the repository and adapt it for your team.

Repository link: [https://github.com/Jaegernauts5103/programming-documentation](https://github.com/Jaegernauts5103/programming-documentation)

---

## Step 1 — Open PowerShell

We recommend using **PowerShell** instead of Command Prompt for better compatibility and path handling.

1. Press **Windows + S**, type **PowerShell**, and open it.  
2. Navigate to the folder where you want the documentation to live. For example, to place it in a `Documentation` folder on your Desktop:

```bash
cd Desktop/Documentation
```

⚠️ If the folder doesn’t exist yet, create it first using:

```bash
mkdir Documentation
cd Documentation
```

---

## Step 2 — Clone the Repository

Use `git clone` to download the repository locally:

```bash
git clone https://github.com/Jaegernauts5103/programming-documentation.git
```

This will create a new folder named `programming-documentation` inside your current directory.

---

## Step 3 — Navigate into the Project

Move into the cloned directory:

```bash
cd programming-documentation
```

You should now see the following structure:

```bash
mkdocs.yml
docs/
  index.md
  // all documentation pages and folders
```

mkdocs.yml
docs/
  index.md

---

## Step 4 — Install Dependencies (if not already done)

Ensure that MKDocs and the Material theme are installed as per the [installation guide](getting-started.md). If you skipped the MKDocs installation, but completed the rest of the installation steps, run:

```bash
pip install mkdocs mkdocs-material
```

---

## Step 5 — Preview the Documentation

Start the MKDocs development server to preview the site locally:

```bash
mkdocs serve
```

Open a browser and go to:

```cpp
http://127.0.0.1:8000
```

... or you can simply `Ctrl + Left Click` the link provided in PowerShell (given you are using PowerShell).

⚠️ If changes don't appear automatically due to auto-reload issues:

1. Go to PowerShell and press `Ctrl + C` to stop the server
2. Restart it with `mkdocs serve`

---

## Step 6 — Update Your Local Copy

To get the latest updates from the GitHub repository in the future:

```bash
git pull origin main
```

This will fetch and merge changes made in the repository.

Another option, if you are using and are familiar with VSCode, you can navigate to the **Source Control** section in the **navigation bar** located on either the left or right side of your screen and push, pull, and fetch changes from there.

---

## Step 7 — Customizing for Your Team

If you are another FRC team using this as a template:

* Rename the project folder if desired.
* Edit `mkdocs.yml` to adjust navigation, theme settings, or project name
* Replace content in the `docs/` folder with your own documentation
* Keep the structure in tact for smooth operation with MKDocs and the Material theme

---

## Notes

* Use PowerShell for these steps on Windows (not required, but **HIGHLY** recommended)
* Regularly pull changes to stay up to date if collaborating with other MECH & Cheese members
* This step ensures a professional, organized documentation workflow for your team