# Foundations of Medical Data Integration

[![Build Status](https://github.com/generated-books/medical-data-integration/workflows/Build%20and%20Deploy%20Jupyter%20Book/badge.svg)](https://github.com/generated-books/medical-data-integration/actions)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

A comprehensive, AI-generated Jupyter Book covering the foundations of medical data integration using Python. This book provides practical training for healthcare data scientists, bioinformaticians, and researchers working with diverse medical datasets.

## 📖 Read the Book

The book is automatically built and deployed at: [https://generated-books.github.io/medical-data-integration](https://generated-books.github.io/medical-data-integration)

## 🤖 AI-Generated Content

**Important Note**: This entire book is AI-generated content. All notebooks, explanations, code examples, and exercises have been created using artificial intelligence. The [`generator.ipynb`](generator.ipynb) file in this repository contains all the code and prompts used for generating the complete book.

## 📚 What's Covered

This book covers the complete pipeline of medical data integration, including:

- **Foundation**: Files, paths, metadata, and storage systems
- **Data Formats**: CSV, Parquet, Arrow, HDF5, Zarr, and medical imaging formats
- **Medical Imaging**: DICOM, OME-TIFF, NIfTI processing and conversion
- **Clinical Data**: NLP, de-identification, vocabulary mapping
- **Advanced Topics**: Entity resolution, parallel processing, longitudinal data analysis

## 🛠 Building the Book Locally

### Prerequisites

- Python 3.8 or higher
- Git

### Quick Start

1. **Clone the repository**
   ```bash
   git clone https://github.com/generated-books/medical-data-integration.git
   cd medical-data-integration
   ```

2. **Create a virtual environment**
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   ```

3. **Install dependencies**
   ```bash
   pip install jupyter-book
   pip install -r docs/requirements.txt
   ```

4. **Build the book**
   ```bash
   cd docs
   jupyter-book build .
   ```

5. **View the book**
   ```bash
   # Open docs/_build/html/index.html in your browser
   # Or serve it locally:
   python -m http.server 8000 --directory _build/html
   ```

### Development Mode

For continuous building during development:

```bash
cd docs
jupyter-book build . --builder html --all
```

To clean previous builds:

```bash
jupyter-book clean .
```

## 📁 Repository Structure

```
├── docs/                    # Jupyter Book source
│   ├── *.ipynb             # Individual notebook chapters
│   ├── intro.md            # Book introduction
│   ├── _config.yml         # Jupyter Book configuration
│   ├── _toc.yml           # Table of contents
│   └── requirements.txt    # Python dependencies
├── generator.ipynb         # AI generation code
├── icon.png               # Book icon
└── README.md              # This file
```

## 🚀 Automatic Deployment

The book is automatically built and deployed using GitHub Actions whenever changes are pushed to the main branch. The workflow file is located at `.github/workflows/deploy.yml`.

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🤝 Contributing

Since this is an AI-generated book, contributions should focus on:
- Reporting errors or issues
- Suggesting improvements to the generation process
- Adding new prompts or topics to the generator

Please open an issue or submit a pull request if you find any problems.

## 📞 Support

If you encounter any issues while building or using this book, please:
1. Check the [Issues](https://github.com/generated-books/medical-data-integration/issues) page
2. Create a new issue with detailed information about the problem
3. Include your Python version, operating system, and error messages