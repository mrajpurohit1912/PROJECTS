# ml-dl-playground Repository

This repository contains multiple Machine Learning and Deep Learning projects.  
Each project is independent and has its own `pyproject.toml` file for dependencies.

## 📂 Repository Structure
```bash
ml_dl_projects/
│── 1_customer_churning/       # Project 1
│   ├── notebooks/             # Jupyter notebooks
│   ├── main.py                # Entry script
│   ├── pyproject.toml         # Dependencies
│
│── 2_project_name/            # Project 2 (example)
│   ├── ...
│
├── README.md                  # Repo documentation
├── Data                       # Data for projects
```

## 📥 Clone the Repository

To clone the entire repo:
```bash
git clone https://github.com/your-username/ml_dl_projects.git
cd ml_dl_projects
```

## 📥 Clone a Specific Project

To clone only one folder (e.g., `1_customer_churning`), use sparse checkout:

```bash
git clone --no-checkout https://github.com/your-username/ml_dl_projects.git
cd ml_dl_projects
git sparse-checkout init --cone
git sparse-checkout set 1_customer_churning

```
## ▶️ Running a Project

Each project is standalone. Example:

```bash
cd 1_customer_churning

# Create virtual environment
python -m venv .venv
source .venv/bin/activate   # Linux/Mac
.venv\Scripts\activate      # Windows

# Install dependencies
pip install .
# OR
poetry install

# Run
python main.py

```

### 📝 Notes / Extra Info

- Use separate virtual environments for each project.  
- Each project may contain datasets in the `data/` folder and notebooks in `notebooks/`.  
- You can contribute by adding new projects following the same structure.  
