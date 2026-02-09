# PDF Learning Repository Setup

## Requirements

- Git
- GitHub CLI (`gh`)
- Authenticated via `gh auth login`

## Steps

### 1. Create Project

```zsh
mkdir pdf-learning-repo
cd pdf-learning-repo
git init
git branch -M main
```

### 2. Directory Structure

```
pdf-learning-repo/
├── pdfs/
├── docs/
├── README.md
└── SETUP.md
```

### 3. Add PDFs

Place all PDF files inside the `pdfs/` directory.

### 4. GitHub Pages

PDFs are copied into `docs/` and listed in `docs/index.html`.

### 5. Create Repository on GitHub

```zsh
gh repo create pdf-learning-repo \
 --public \
 --source=. \
 --remote=origin \
 --push
```

### 6. Enable Pages

- Go to **Settings → Pages**
- Source: **main**
- Folder: **/docs**

## Result

GitHub Pages URL:

```
https://srirampeddapanta.github.io/pdf-learning-repo/
```
