## Installing MKDocs and Material for MKDocs

Installing **MKDocs** is a bit different from installing normal
applications. Instead of downloading a program or using an app store,
MKDocs is installed through the **command line** using Python's package
manager, `pip`.

Team **MECH & Cheese** uses MKDocs along with the **Material for
MKDocs** theme to create clean, organized, and professional
documentation. This guide walks you through installing everything you
need to get started.

---

## Prerequisites

Before installing MKDocs, make sure the following are installed:

-   **Python 3.8 or later**
-   **pip**, which is included with most Python installations

To verify that Python is installed, run:

``` bash
python --version
```

or:

``` bash
python3 --version
```

If Python is not installed, download it from:
[https://www.python.org/downloads/](https://www.python.org/downloads/)

### Recommended Terminal

While MKDocs works in any command-line environment, **we strongly recommend using PowerShell** instead of Command Prompt. PowerShell handles paths, Python commands, and MKDocs processes more reliably, especially when working with virtual environments or the Material theme.

---

## Step 1 — Install MKDocs

Once Python and pip are ready, install MKDocs by running:

``` bash
pip install mkdocs
```

To confirm that MKDocs installed correctly:

``` bash
mkdocs --version
```

---

A version number means you're good to go.

## Step 2 — Install Material for MKDocs

MECH & Cheese uses the **Material for MKDocs** theme for its clean
layout, ease of customization, and powerful features.

Install it using:

``` bash
pip install mkdocs-material
```

You can confirm both packages were installed by running:

``` bash
pip list
```

Look for:

-   `mkdocs`
-   `mkdocs-material`

---

## Step 3 — Create a New MKDocs Project

Before creating the project, navigate to the folder where you want your documentation to live.
For example, if you want it inside a `Documentation` folder on your desktop:

``` bash
cd Desktop/Documentation
```

Once you are in the correct location, create a new documentation project by running:

``` bash
mkdocs new my-project
```

Then move into the project folder:

``` bash
cd my-project
```

Inside, you should see:

    mkdocs.yml
    docs/
      index.md

---

## Step 4 — Start the Local Development Server

MKDocs includes a built-in development server that automatically reloads
when you save changes. However, Team MECH & Cheese has noticed that
auto-reload does not always work consistently on Windows. If your page
does not update automatically, don’t worry — this is normal.

Start the server by running:

```bash
mkdocs serve
```

Then visit this address in your browser:

```
127.0.0.1:8000
```

### If auto-reload stops working  
Sometimes MKDocs will freeze and stop detecting changes. To fix this:

1. Go to your PowerShell window  
2. Press **Ctrl + C** to stop the server  
3. Restart the server with:  

```bash
mkdocs serve
```

This refreshes the build and forces the latest version of the site to appear. You may need to do this frequently while editing.

---

## Step 5 — Enable the Material Theme

To switch your site to Material for MKDocs, open the `mkdocs.yml` file
and modify the `theme:` section as follows:

``` yaml
theme:
  name: material
```

Save the file and refresh your browser --- your documentation will now
use the Material theme.

---

## Installation Complete

You now have:

-   MKDocs installed
-   Material for MKDocs enabled
-   A working documentation project
-   A live development server

You are ready to begin building MECH & Cheese's documentation using
professional, modern tools.

Recommended next steps include:

-   Setting up a standard project structure
-   Creating navigation and sidebar layouts
-   Learning Markdown formatting basics
-   Customizing the Material theme
-   Writing your first full documentation page
