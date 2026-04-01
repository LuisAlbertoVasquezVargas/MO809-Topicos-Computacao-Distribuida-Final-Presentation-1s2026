
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

### 🛠️ Build Instructions

#### Option A: Overleaf (Cloud - Beginner Friendly)
1. Create a new project in Overleaf  
2. Copy and paste `src/main.tex`  
3. Click **Recompile**

---

#### Option B: Local Setup (Arch Linux - Fast & Minimal)

##### 1. Install dependencies
```bash
sudo pacman -S texlive-basic texlive-latexextra texlive-fontsrecommended \
               texlive-fontsextra texlive-bibtexextra texlive-plaingeneric \
               texlive-binextra texlive-science zathura zathura-pdf-mupdf biber
````

---

##### 2. Live development (auto-compile + auto-refresh)

Start the compiler (watch mode):

```bash id="7y7hzt"
latexmk -pdf -pvc -outdir=outputs src/main.tex
```

In another terminal, open the PDF viewer:

```bash id="3z7n7b"
zathura outputs/main.pdf
```

---

### ⚡ Workflow

* Edit in **Neovim**
* Save file (`:w`)
* PDF updates automatically in Zathura

No plugins required. Fast feedback loop.

---

### 📂 Repository Structure

```id="6hskds"
.
├── src/
│   └── main.tex
├── outputs/
│   └── main.pdf    # generated presentation
└── README.md
```

---

### 🎨 Design Standards

* **Color Palette:** Space Indigo (`#141B41`), Ocean Deep (`#306BAC`)
* **Editor:** Neovim (plugin-free workflow)
* **Convention:** Each `.tex` file must include its relative path as a comment on the first line

---

### 🚀 Performance Note

Compared to Overleaf, local compilation with `latexmk` provides near-instant feedback, making it significantly more efficient for iterative slide editing and final adjustments.

