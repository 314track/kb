---
title: "pip"
---

# pip

Upgrade pip

```bash
python3 -m pip install --upgrade pip
```

Upgrade all packages in venv

```bash
pip freeze > requirements.txt
```

```bash
pip install -r requirements.txt --upgrade --force
```

Write all installed packages in current venv into `requirements.txt`

```bash
pip freeze > requirements.txt
```
Install all listed packages in `requirements.txt` into current venv

```bash
pip install -r requirements.txt
```
