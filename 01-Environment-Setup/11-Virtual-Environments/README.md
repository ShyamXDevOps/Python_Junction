# Virtual Environments

> Part of [Module 01 — Python Environment Setup](../README.md).

A virtual environment isolates packages for one project from other projects and the base interpreter.

## Ubuntu / WSL

```bash
mkdir -p ~/projects/python-environment-demo
cd ~/projects/python-environment-demo

python3 -m venv .venv
source .venv/bin/activate
```

Verify the environment:

```bash
which python
python --version
python -m pip --version
```

Install a package:

```bash
python -m pip install requests
```

Deactivate:

```bash
deactivate
```

## Windows PowerShell

```powershell
python -m venv .venv
.\.venv\Scripts\Activate.ps1
python --version
deactivate
```

## Windows Command Prompt

```cmd
.venv\Scriptsctivate.bat
```

## Remove an environment

Deactivate it first, then remove the `.venv` directory. It can be recreated from the project's dependency declarations.

## Record dependencies

```bash
python -m pip freeze > requirements.txt
python -m pip install -r requirements.txt
```

`requirements.txt` is a common way to record exact installed package versions for a simple project. More complex projects may use additional dependency-management and lock-file tools.

Reference: [venv documentation](https://docs.python.org/3/library/venv.html)
