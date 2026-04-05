<!-- README.md -->

# MO809 - Tópicos em Computação Distribuída

## Final Presentation - 1s2026

**Project:** A Data Structure Perspective to the RDD-based Apriori Algorithm on Spark

---

### 📝 Description
This repository contains the LaTeX source code and final presentation for the **MO809** course at **UNICAMP**. The presentation analyzes computational bottlenecks of the Apriori algorithm in distributed systems (Apache Spark) and compares different data structures used for candidate matching within Resilient Distributed Datasets (RDDs).

---

### 👤 Author
- **Luis Alberto Vásquez Vargas** (Master's Student @ IC-UNICAMP)  
- **Professor:** Luiz Fernando Bittencourt  

---

### 🛠️ Build Instructions (Arch Linux)

#### 1. Install dependencies
```bash
sudo pacman -S texlive-basic texlive-latexextra texlive-fontsrecommended \
               texlive-fontsextra texlive-bibtexextra texlive-plaingeneric \
               texlive-binextra texlive-science zathura zathura-pdf-mupdf \
               latexmk
```

#### 2. One-Line Build & Watch
Run this from the project root. It prepares the output mirror, cleans old artifacts, and starts the live-recompile loop:

```bash
mkdir -p outputs/sections outputs/style && rm -rf outputs/* && \
TEXINPUTS=./src//:./img//: latexmk -pdf -pvc -outdir=outputs src/main.tex
```

#### 3. Open Preview
Run this in a separate terminal:

```bash
zathura outputs/main.pdf
```

---

### ⚡ Workflow
* Edit modules in **Neovim** (e.g., `src/sections/03_the_problem.tex`).
* Save file (`:w`).
* `latexmk` detects the change via recursive search (`//`) and updates the PDF in `outputs/`.
* **Zathura** refreshes the view instantly.

---

### 📂 Repository Structure
```text
.
├── img/                # Graphics and author photos
├── outputs/            # Build artifacts (mirrors src structure)
│   └── main.pdf        # Final rendered presentation
├── src/
│   ├── main.tex        # Entry point (Executive Controller)
│   ├── sections/       # Content modules (.tex)
│   └── style/          # Preamble and theme configuration
└── README.md
```

---

### 🎨 Design Standards
* **Color Palette:** Space Indigo (`#141B41`), Ocean Deep (`#306BAC`)
* **Editor:** Neovim (plugin-free workflow)
* **Convention:** Every `.tex` file **must** include its relative filepath at the very first line followed by an empty line.

