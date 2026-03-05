# SOFTWARE REQUIREMENTS SPECIFICATION 
# BeatFinder: Intelligent Music Discovery & Recommendation Platform 


## Repository Structure

```
.
├── main.tex          # Main LaTeX source file
├── figures/          # All embedded images
│   ├── figure1.png
│   ├── figure2.png
│   └── ...
└── README.md
```

## How to Compile

### Option 1 — Overleaf (online, no install needed) (Recommended)

1. Go to [overleaf.com](https://www.overleaf.com) and create a free account.
2. Click **New Project → Upload Project**.
3. Zip this entire folder (including `figures/`) and upload the zip.
4. Overleaf will auto-detect `main.tex` and compile it to pdf — click **Recompile**.

### Option 2 — Command Line

Make sure you have a LaTeX distribution installed:
- **Windows**: [MiKTeX](https://miktex.org/) or [TeX Live](https://tug.org/texlive/)
- **macOS**: [MacTeX](https://www.tug.org/mactex/)
- **Linux**: `sudo apt install texlive-full`

Then compile:

```bash
pdflatex main.tex   # Run once
pdflatex main.tex   # Run a second time to resolve cross-references
```

This produces `main.pdf` in the same folder.


### Option 3 — VS Code

1. Install the [LaTeX Workshop](https://marketplace.visualstudio.com/items?itemName=James-Yu.latex-workshop) extension.
2. Open the project folder in VS Code.
3. Open `main.tex` and press `Ctrl+Alt+B` (or `Cmd+Alt+B` on Mac) to build.


## Notes

- Images are referenced relative to `figures/` — **do not move them**.
- Run `pdflatex` **twice** to ensure all labels and references are resolved.
