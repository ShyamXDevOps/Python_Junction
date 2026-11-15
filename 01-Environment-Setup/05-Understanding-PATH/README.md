# Understanding PATH

> Part of [Module 01 — Python Environment Setup](../README.md).

`PATH` is an environment variable containing directories searched by the shell when a command is entered without a full path.

## Linux / WSL

```bash
echo "$PATH"
command -v python3
which -a python3
```

## Windows PowerShell

```powershell
$env:Path -split ';'
Get-Command python -All
```

## Check the interpreter from Python

```python
import sys

print(sys.executable)
print(sys.version)
```

When multiple Python installations exist, the first matching command in the search order may be selected. Diagnose the resolved path before changing PATH.

## Exercise

Find the Python executable in both Windows and WSL. Compare the paths and explain why they are different.
