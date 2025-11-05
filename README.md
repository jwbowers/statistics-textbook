# Statistical Thinking Through Exploration

**A Discovery-Based Approach to Applied Statistics for the Social Sciences**

By Jake Bowers

## About This Book

This textbook emerged from over a decade of teaching graduate statistics using a flipped classroom approach. Instead of lectures followed by problem sets, students **explore** statistical concepts through data and code *before* class, then come to discuss what they discovered and what puzzled them.

The approach draws on the pedagogical philosophies of Paulo Freire, Maria Montessori, and John Dewey, emphasizing:

- **Active learning** through hands-on exploration
- **Question-driven** rather than lecture-driven instruction
- **Simulation-based** understanding of concepts
- **Critical evaluation** of statistical methods through operating characteristics

## Structure

The book is organized into seven parts:

- **Part I**: The Pedagogy of Statistical Discovery
- **Part II**: Three Cheers for Description
- **Part III**: Two Cheers for Statistical Inference
- **Part IV**: One Cheer for Causal Inference
- **Part V**: Adjustment - Controlling For What?
- **Part VI**: Large Sample Theory and Connections
- **Part VII**: Model-Based Inference

## Viewing the Book

**Online version**: https://[your-github-username].github.io/statistics-textbook

**PDF version**: Available in the Releases section

## Building the Book Locally

### Prerequisites

1. Install [R](https://cran.r-project.org/) (version 4.0+)
2. Install [Quarto](https://quarto.org/docs/get-started/)
3. Install required R packages:

```r
install.packages(c(
  "tidyverse", "here", "knitr", "broom",
  "estimatr", "DeclareDesign", "optmatch",
  "RItools", "coin", "boot", "sandwich", "lmtest"
))
```

### Building

**HTML version:**

```bash
quarto render
```

The output will be in the `_book/` directory.

**PDF version:**

```bash
quarto render --to pdf
```

Note: PDF rendering requires LaTeX (e.g., TinyTeX):

```bash
quarto install tinytex
```

**Single chapter:**

```bash
quarto render chapters/01-description-1d.qmd
```

## Repository Structure

```
statistics-textbook/
├── _quarto.yml           # Book configuration
├── index.qmd             # Preface
├── chapters/             # Book chapters
│   ├── 00-introduction.qmd
│   ├── 01-description-1d.qmd
│   └── ...
├── data/                 # Data files
├── images/              # Figures and images
├── css/                 # Custom styling
├── references.bib       # Bibliography
└── README.md           # This file
```

## For Students

### How to Use This Book

1. **Read** the scenario at the start of each chapter
2. **Work through** the exploration code (run every line yourself!)
3. **Answer** the embedded questions
4. **Experiment**: modify code, try your own data
5. **Discuss**: in study groups or class
6. **Extend**: apply to your own research

See the "How to Use This Book" chapter for detailed guidance.

### Getting Help

- **Technical issues**: Open an issue on GitHub
- **Statistical questions**: See the recommended readings in each chapter
- **General questions**: Check the FAQ in the appendices

## For Instructors

### Using This Book in Your Course

This book is designed for a flipped classroom but can be adapted to other formats. See the "How to Use This Book" chapter for guidance on:

- Weekly schedules
- Class activities
- Assessment strategies
- Customization options

### Teaching Materials

Additional materials for instructors (slides, answer keys, additional exercises) are available in the `teaching-materials/` branch (private, request access).

## Contributing

Contributions are welcome! Whether you've found a typo, have a suggestion for improving an explanation, or want to contribute a new exercise:

1. Fork this repository
2. Make your changes
3. Submit a pull request

See CONTRIBUTING.md for guidelines.

## License

### Book Content

The text and content of this book is licensed under [Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International](https://creativecommons.org/licenses/by-nc-sa/4.0/).

You are free to:

- Share and adapt the material
- Use it for teaching

Under the following terms:

- Give appropriate credit
- Non-commercial use only
- Share adaptations under the same license

### Code

All code (both in the book and in the repository) is licensed under the [MIT License](LICENSE-CODE).

You are free to use the code for any purpose, including commercial purposes.

## Citation

If you use this book in your teaching or research, please cite:

```bibtex
@book{bowers2025statistics,
  title={Statistical Thinking Through Exploration: A Discovery-Based Approach to Applied Statistics},
  author={Bowers, Jake},
  year={2025},
  url={https://github.com/[your-username]/statistics-textbook},
  note={Online open-access textbook}
}
```

## Acknowledgments

This book would not exist without:

- The hundreds of students who worked through these explorations and asked challenging questions
- The methods preceptors who provided invaluable feedback
- The scholars whose work we build upon (especially Paul Rosenbaum, David Cox, Andrew Gelman, and many others)
- The open-source community that created R, Quarto, and the many packages we use

## Contact

- **Author**: Jake Bowers
- **Email**: jwbowers@illinois.edu
- **Website**: http://jakebowers.org/
- **Issues**: Please use GitHub issues for questions and bug reports

---

**Note to Jake**: This README can be customized with your actual GitHub username, website URL, and other specific details once you've set up the repository.
