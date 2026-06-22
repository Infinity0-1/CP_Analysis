# Analysis Course Notes

This repository contains our Analysis course notes written in LaTeX.

## Repository Structure

```text
.
├── main.tex
└─── Chapters
    ├── Chapter 1.tex
    ├── Series 1.tex
    ├── Chapter 2.tex
    ├── Series 2.tex
    ├── Chapter 3.tex
    ├── ...
    ├── ...
```

* `main.tex` is the main document and should be used to compile the final PDF.
* `Chapters/Chapteer 1.tex` contains Chapter 1.
* `Chapters/Chapter 2.tex` contains Chapter 2.
* `Chapters/Series 1.tex` contains Series 1 and its solutions.
* `Chapters/Series 2.tex` contains Series 2 and its solutions.

Additional chapter files may be added as the course progresses.

## Building the PDF

Compile the document from the repository root:

```bash
pdflatex main.tex
```

If multiple passes are required:

```bash
pdflatex main.tex && pdflatex main.tex
```

## Collaboration Workflow

Before starting work:

```bash
git pull
```

After making changes on a new branch:

```bash
git add .
git commit -m "Describe your changes"
git push -u origin new_branch
```

## Editing Rules

1. Do not modify another person's work without discussing it first.
2. Keep each chapter in its corresponding file inside the `Chapters` directory.
3. Ensure that `main.tex` compiles successfully before pushing changes.
4. Write clear and consistent mathematical notation.
5. Use LaTeX environments whenever appropriate (`theorem`, `proof`, `definition`, etc.).

## Example Workflow

```bash
git pull

# Edit chapter files on a new branch

git add .
git commit -m "Added notes on continuity"
git push -u origin new_branch
```
Then, open a pull request on GitHub.
