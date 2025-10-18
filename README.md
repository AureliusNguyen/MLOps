# MLOps Lectures

A multi-lecture workspace for hands-on MLOps. Each **lecture** is its own mini-project with an isolated virtual environment and Jupyter kernel.

## Structure
```
.
├── LectureN/
│   ├── notebooks/
│   ├── scripts/
│   ├── configs/
│   ├── data/           # gitignored
│   └── requirements.txt
└── README.md
```

## Quick Start (per lecture)
```bash
cd LectureN
python -m venv .venv
source .venv/bin/activate
python -m pip install -U pip ipykernel
pip install -r requirements.txt
NAME="$(basename "$PWD")"
python -m ipykernel install --user --name "${NAME}-venv" --display-name "Python (${NAME})"
```
