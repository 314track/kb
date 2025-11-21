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
pip list --outdated | cut -d ' ' -f1 | tail -n +3 | xargs -I {} pip install -U "{}"
```

Export and import packages

```bash
pip freeze > requirements.txt
```

```bash
pip install -r requirements.txt --upgrade
```

Write all installed packages in current venv into `requirements.txt`

```bash
pip freeze > requirements.txt
```
Install all listed packages in `requirements.txt` into current venv

```bash
pip install -r requirements.txt
```
