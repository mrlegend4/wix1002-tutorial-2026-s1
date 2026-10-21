# WIX1002 Tutorials — 2026 Semester 1

Chua Jun Yu OCC3
Tutorial materials for **WIX1002 Fundamentals of Programming**. Each tutorial has its own folder containing the original question PDF. Create your answers in Markdown in your own fork of this repository.

## Tutorial list

| Tutorial | Topic | Questions | Your answer file (create in your fork) |
| --- | --- | --- | --- |
| 01 | Problem Solving in Programming | [PDF](tutorial-01/T-1002-01.pdf) | `tutorial-01/answers.md` |
| 02 | Java Fundamental | [PDF](tutorial-02/T-1002-02.pdf) | `tutorial-02/answers.md` |
| 03 | Flow of Control (Selection) | [PDF](tutorial-03/T-1002-03.pdf) | `tutorial-03/answers.md` |
| 04 | Flow of Control (Repetition) | [PDF](tutorial-04/T-1002-04.pdf) | `tutorial-04/answers.md` |
| 05 | Arrays | [PDF](tutorial-05/T-1002-05.pdf) | `tutorial-05/answers.md` |
| 06 | Java Methods | [PDF](tutorial-06/T-1002-06.pdf) | `tutorial-06/answers.md` |
| 07 | File Input and Output | [PDF](tutorial-07/T-1002-07.pdf) | `tutorial-07/answers.md` |
| 08 | Class | [PDF](tutorial-08/T-1002-08.pdf) | `tutorial-08/answers.md` |
| 09 | Inheritance | [PDF](tutorial-09/T-1002-09.pdf) | `tutorial-09/answers.md` |
| 10 | Polymorphism | [PDF](tutorial-10/T-1002-10.pdf) | `tutorial-10/answers.md` |

## Student guide

### 1. Prepare your tools

You need a [GitHub account](https://github.com/signup), [Git](https://git-scm.com/downloads), and a text editor such as VS Code. Use Terminal on macOS/Linux or Git Bash on Windows for the commands below.

Check that Git is installed:

```bash
git --version
```

### 2. Fork this repository

1. Sign in to GitHub and open [FSKTMCoders/wix1002-tutorial-2026-s1](https://github.com/FSKTMCoders/wix1002-tutorial-2026-s1).
2. Click **Fork** near the top right.
3. Select your own GitHub account as the owner and keep the repository name `wix1002-tutorial-2026-s1`.
4. Click **Create fork**.
5. Check that the address now starts with `https://github.com/YOUR-USERNAME/`.

Your fork is your own repository where you will save your answers.

### 3. Clone your fork to your computer

Replace `YOUR-USERNAME` with your actual GitHub username before running:

```bash
git clone https://github.com/YOUR-USERNAME/wix1002-tutorial-2026-s1.git
cd wix1002-tutorial-2026-s1
git remote -v
```

Check that `origin` points to **your username's repository** for both fetch and push. If you accidentally cloned the course repository, correct the remote:

```bash
git remote set-url origin https://github.com/YOUR-USERNAME/wix1002-tutorial-2026-s1.git
git remote -v
```

### 4. Set your Git commit identity

Run these commands inside the cloned repository, replacing the example values with your own name and a verified GitHub email address (or your GitHub-provided no-reply address):

```bash
git config user.name "Your Name"
git config user.email "your-email@example.com"
```

These values identify your commits; they do not sign you in to GitHub.

### 5. Create a Markdown answer file for each tutorial

Open the cloned repository in your editor. Read the PDF in `tutorial-01`, then create a new file named **`answers.md`** inside that same folder. Ensure the filename ends in `.md`, not `.md.txt`.

Use this structure as a starting point:

````markdown
# Tutorial 01 — Answers

## Part I

### Question 1

Write your answer and explanation here.

### Question 2

Write your answer here.

## Part II

### Question 1

Write your answer here.
````

Match the parts, question numbers, and subparts in the PDF. Add a heading for every question and subpart you answer; the example above is only a starting structure.

For Java answers, use a fenced code block:

````markdown
```java
// Write your Java answer here.
```
````

Use `text` code blocks for pseudocode or program output, and Markdown tables for IPO models. For flowcharts, you can use a [Mermaid diagram](https://docs.github.com/en/get-started/writing-on-github/working-with-advanced-formatting/creating-diagrams) in Markdown or save an image in the same tutorial folder and embed it with `![Flowchart](flowchart.png)`.

Keep the question PDFs in place. Save your work and preview the Markdown to check headings, code blocks, tables, and diagrams.

### 6. Review, stage, and commit your answers

From the repository's root folder, review your changes:

```bash
git status
git diff -- tutorial-01/answers.md
```

For a new, untracked file, `git diff` will not show its contents yet. Stage the file, then review the staged version before committing:

```bash
git add tutorial-01/answers.md
git diff --cached
git commit -m "Add Tutorial 01 answers"
```

If you created a flowchart image, stage it too before committing, for example `git add tutorial-01/flowchart.png`.

### 7. Push the commit to your own repository

Confirm the destination and upload your commit:

```bash
git remote -v
git push origin main
```

Authenticate with GitHub if prompted. For HTTPS, use a credential manager or personal access token when needed; your GitHub account password cannot authenticate Git pushes. Follow [GitHub's HTTPS authentication guide](https://docs.github.com/en/get-started/git-basics/about-remote-repositories#cloning-with-https-urls) if authentication fails.

Open your fork on GitHub, select `main`, and check that `tutorial-01/answers.md` appears and renders correctly. A commit saves your work locally; a push uploads that commit to GitHub.

### 8. Repeat for Tutorials 02–10

Create a separate `answers.md` inside each corresponding tutorial folder. For example, after answering Tutorial 02:

```bash
git add tutorial-02/answers.md
git diff --cached
git commit -m "Add Tutorial 02 answers"
git push origin main
```

Repeat the same process when revising an existing answer. When all tutorials are complete, your fork should contain `tutorial-01/answers.md` through `tutorial-10/answers.md`, alongside the original PDFs. Your answers remain in your own fork; no pull request is required by this guide.

For more help, see GitHub's guides to [forking a repository](https://docs.github.com/en/pull-requests/how-tos/work-with-forks/fork-a-repo?tool=webui) and [pushing commits](https://docs.github.com/en/get-started/using-git/pushing-commits-to-a-remote-repository).
