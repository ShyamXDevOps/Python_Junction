# Installing Python on Ubuntu

> Part of [Module 01 — Python Environment Setup](../README.md).

First check the existing Python installation:

```bash
python3 --version
command -v python3
```

Install Python and common development components only if needed:

```bash
sudo apt update
sudo apt install -y python3 python3-pip python3-venv
```

Verify:

```bash
python3 --version
python3 -m pip --version
python3 -m venv --help
```

## Important system Python guidance

Ubuntu uses Python for some system tools. Do not replace the OS-managed interpreter or use `sudo pip` to install project packages globally. Use `apt` for OS-managed packages and a virtual environment for project dependencies.

## Exercise

Record the Python version and executable path on your Ubuntu machine.
