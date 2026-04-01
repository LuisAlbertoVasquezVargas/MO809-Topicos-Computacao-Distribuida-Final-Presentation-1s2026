
# MO809 - Tópicos em Computação Distribuída
## Final Presentation - 1s2026

**Project:** A Data Structure Perspective to the RDD-based Apriori Algorithm on Spark

### 📝 Description
This repository contains the LaTeX source code and final presentation for the **MO809** course at **UNICAMP**. The presentation analyzes the computational bottlenecks of the Apriori algorithm in distributed systems (Apache Spark) and compares different data structures used for candidate matching within Resilient Distributed Datasets (RDDs).

### 👤 Author
- **Luis Alberto Vásquez Vargas** (Master's Student @ IC-UNICAMP)
- **Professor:** Luiz Fernando Bittencourt

### 🛠️ Build Instructions

#### Option A: Overleaf (Cloud - Beginner Friendly)
This is the easiest way to get started without installing any software:
1. Create a new project in **Overleaf**.
2. **Copy and paste** the content of `src/main.tex` into the Overleaf editor.
3. Hit **Recompile**.

#### Option B: Local Setup (Omarchy / Arch Linux - Professional Speed)
For a faster, near-instant editing experience on your laptop:

1. **Install Dependencies:**
   ```bash
   sudo pacman -S texlive-basic texlive-latexextra texlive-fontsrecommended \
                  texlive-fontsextra texlive-bibtexextra texlive-plaingeneric \
                  texlive-binextra texlive-science zathura zathura-pdf-mupdf biber
   ```

2. **Live Development (Continuous Mode):**
   Run the following command in your terminal to auto-compile and refresh the PDF every time you save in **Neovim**:
   ```bash
   latexmk -pvc -pdf src/main.tex
   ```

### 📂 Repository Structure
- `src/main.tex`: Beamer source code (Madrid theme with custom Space Indigo palette).
- `.latexmkrc`: Local configuration for automated builds (Zathura integration).
- `README.md`: Project documentation.

### 🎨 Design Standards
- **Color Palette:** Space Indigo (`#141B41`) and Ocean Deep (`#306BAC`).
- **Editor:** Neovim + VimTeX for local live synchronization.
- **Coding Standard:** Every `.tex` file must include the relative filepath as a comment on the first line.

---

### 🚀 Performance Note
While Overleaf is great for collaboration, local compilation using `latexmk` on this setup provides near-instant feedback, significantly reducing the "edit-sync-view" cycle time during final slide adjustments for your UNICAMP presentation.
