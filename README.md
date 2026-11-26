# SYSTEM-Rewrite
A passion Project made among friends, this will be used for us to quickly manage things


### Prerequisites

Before starting, you need:

* A free **GitHub account** (and collaborator access if your repository is Private, added under **Settings > Collaborators**).
* Either **GitHub Desktop** (easiest for artists and writers) or **Git** (for command-line / VS Code users).
* **Ren'Py Launcher** installed to open and test the project folder.

---

### Method 1: Using GitHub Desktop 

#### 1. Clone the Repository to Your Computer

1. Open **GitHub Desktop** and sign in with your GitHub account.
2. Go to **File > Clone Repository**.
3. Select the **SYSTEM-Rewrite** repository from the list (or paste its URL under the **URL** tab).
4. Choose a local folder path on your computer (for example, inside your Ren'Py projects directory) and click **Clone**.
*Verification:* The full project folder with scripts and assets appears inside the chosen folder on your computer.

#### 2. Open and Edit the Project

1. Launch **Ren'Py**, click **Preferences > Projects Directory** (if needed) to point to the parent folder, and select the cloned project to run or test it.
2. Add new art/audio assets into the `game/` subfolders or edit `.rpy` scripts in your editor as usual.

#### 3. Upload Your Changes Back to GitHub

1. Before starting work each day, open **GitHub Desktop** and click **Fetch origin** (then **Pull origin** if updates exist) so you have everyone else's latest edits.
2. After saving your work, return to **GitHub Desktop**—your modified and added files appear on the left under **Changes**.
3. Type a short description in the **Summary** box at the bottom-left (e.g., `Added sprite variants` or `Updated chapter 1 dialogue`) and click **Commit to main**.
4. Click **Push origin** in the top bar to upload your commit to GitHub.
*Verification:* The **Push origin** button changes back to **Fetch origin**, and your new files appear on the GitHub website when you refresh the page.

---

### Method 2: Using the Terminal / VS Code

#### 1. Clone the Repository

Open a terminal in the folder where you store your Ren'Py projects and run:

```bash
git clone https://github.com/solacsticey/SYSTEM-Rewrite.git
cd SYSTEM-Rewrite

```

*Verification:* Running `dir` (Windows) or `ls` (Mac/Linux) lists the project files inside `SYSTEM-Rewrite`.

#### 2. Daily Workflow (Pull, Edit, Commit, Push)

1. **Get latest changes before editing:**
```bash
git pull origin main

```


2. **Edit scripts or add assets** inside the folder and test in Ren'Py.
3. **Stage, commit, and upload your changes:**
```bash
git add .
git commit -m "Describe what you changed"
git push origin main

```


*Verification:* The terminal finishes without `[rejected]` errors and displays `main -> main`.

---

### Quick Rule

* **Always pull before you start:** Pulling first prevents overwritten work and merge conflicts.
* **Avoid editing the same `.rpy` file at the same time:** Coordinate who is editing `script.rpy` or split scenes into separate `.rpy` files (e.g., `scene1.rpy`, `scene2.rpy`).
* **Keep individual files under 100 MiB:** Export final web/game-ready PNGs, WEBPs, or OGGs rather than huge raw source files.
