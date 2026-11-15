# Troubleshooting Python Setup

> Part of [Module 01 — Python Environment Setup](../README.md).

Diagnose before reinstalling.

| Error / symptom | Check | Next step |
|---|---|---|
| `python: command not found` on Linux | `command -v python3` | Try `python3`; install distro package if absent |
| Python opens Microsoft Store | `Get-Command python -All` | Inspect app execution aliases and installation |
| Wrong version runs | `sys.executable`, `where.exe python` | Inspect PATH and selected interpreter |
| `No module named venv` | Check Ubuntu packages | Install `python3-venv` with apt |
| pip permission denied | `python -m pip --version` | Create and activate a virtual environment |
| externally managed environment | Check active interpreter | Use a venv; do not force global installation |
| VS Code cannot find Python | Select Interpreter | Choose installed interpreter or project `.venv` |
| PowerShell activation blocked | Read full policy error | Use cmd activation or approved user-scoped policy |
| `code` not found in WSL | `command -v code` | Check VS Code WSL extension/setup |

## Useful diagnostic commands

### Linux / WSL

```bash
python3 --version
command -v python3
which -a python3
python3 -m pip --version
```

### Windows PowerShell

```powershell
python --version
py --version
Get-Command python -All
where.exe python
```

### Inside Python

```python
import sys
print(sys.executable)
print(sys.version)
```

Do not share screenshots containing usernames, access tokens, private paths or other sensitive information.
