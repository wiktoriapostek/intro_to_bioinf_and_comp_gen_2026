# Introduction to Bioinformatics and Computational Genomics - Spring 2026

This repository contains course materials for **Bioinformatics** taught in the Spring 2026 semester at the **MiNI department** (Faculty of Mathematics and Information Science) at **Warsaw University of Technology**.

## 📚 Course Content

The repository includes:
- **Laboratories**: Hands-on exercises and practical assignments
- **Dependencies**: All required Python packages for bioinformatics analysis

## 🛠️ Prerequisites

### Installing uv

This project uses `uv` for fast Python package management. Install it using one of the following methods:

#### Option 1: Using pip
```bash
pip install uv
```

#### Option 2: Using curl (recommended)
```bash
curl -LsSf https://astral.sh/uv/install.sh | sh
```

#### Option 3: Using pipx
```bash
pipx install uv
```

#### Option 4: Using Homebrew (macOS)
```bash
brew install uv
```

## 🚀 Getting Started

### 1. Clone the Repository
```bash
git clone git@github.com:maciek-wisniewski/intro_to_bioinf_and_comp_gen_2026.git
cd intro_to_bioinf_and_comp_gen_2026
```

### 2. Create and Activate Virtual Environment
```bash
# Create virtual environment and install dependencies
uv sync

# Activate the virtual environment
source .venv/bin/activate  # On macOS/Linux
# or
.venv\Scripts\activate     # On Windows
```

### 3. Launch Jupyter Notebook
```bash
# Start Jupyter Notebook server
jupyter notebook

# Or start JupyterLab (alternative interface)
jupyter lab
```

## 📁 Project Structure

```
intro_to_bioinf_and_comp_gen_2026/
├── notebooks/
│   ├── 01-sequences.ipynb
│   ├── 02-alignment.ipynb
│   └── ...
├── pyproject.toml        # Project configuration and dependencies
├── uv.lock              # Locked dependency versions
└── README.md            # This file
```

## 📦 Included Packages

The project includes essential bioinformatics and data science packages:

- **biotite** (≥1.4.0) - Bioinformatics toolkit
- **gemmi** (≥0.7.3) - Crystallography and structural biology
- **jupyter** (≥1.1.1) - Interactive notebooks
- **matplotlib** (≥3.10.6) - Plotting and visualization
- **pandas** (≥2.3.3) - Data manipulation and analysis
- **rdkit** (≥2025.3.6) - Cheminformatics and molecular informatics
- **scikit-learn** (≥1.7.2) - Machine learning
- **seaborn** (≥0.13.2) - Statistical data visualization

## 🔧 Development

### Adding New Dependencies
```bash
# Add a new package
uv add package-name

# Add a development dependency
uv add --dev package-name
```

### Updating Dependencies
```bash
# Update all dependencies
uv sync --upgrade

# Update specific package
uv add package-name@latest
```

### Running the Main Script
```bash
python main.py
```

## 📖 Usage

1. **For Labs**: Navigate to `notebooks/` and work through the exercises
2. **Interactive Development**: Use Jupyter Notebook or JupyterLab for interactive coding

## 📄 License

This project is for educational use in the Bioinformatics course at Warsaw University of Technology.

---

**Course**: Introduction to Bioinformatics and Computational Genomics - Spring 2026  
**Institution**: MiNI Department, Warsaw University of Technology  
**Python Version**: ≥3.11  
**Package Manager**: uv