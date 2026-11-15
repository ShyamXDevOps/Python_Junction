# Installing Python on Windows

> Part of [Module 01 — Python Environment Setup](../README.md).

Use the current official Windows installation instructions. The Python Install Manager is the current recommended route in the Python documentation.

## Install manager with WinGet

Open PowerShell:

```powershell
winget install 9NQ7512CXL7T -e
```

Open a new PowerShell window after installation. Inspect available runtimes:

```powershell
py list
```

Install a supported runtime, for example Python 3.14 if available through the manager:

```powershell
py install 3.14
```

Verify:

```powershell
python --version
py --version
python -m pip --version
```

## Alternative

Use the official downloads page: https://www.python.org/downloads/windows/

Follow the current installer's instructions for PATH and command aliases. Do not add arbitrary directories to PATH.

## Multiple versions

Use the manager's version-selection features when multiple runtimes are needed. Always verify the executable and version used by a project.

Reference: [Official Windows documentation](https://docs.python.org/3/using/windows.html)
