# pip and Package Installation

> Part of [Module 01 — Python Environment Setup](../README.md).

pip installs Python packages into the environment selected by the Python interpreter.

Check pip:

```bash
python3 -m pip --version
```

Inside an activated virtual environment:

```bash
python -m pip install requests
python -m pip show requests
python -m pip list
```

Use `python -m pip` rather than relying on a bare `pip` command; this makes the interpreter association explicit.

On Ubuntu, system Python may be externally managed. Use a virtual environment rather than bypassing that protection for normal project work.

Check packages before installing them: package name similarity is not proof of trustworthiness.

References: https://pip.pypa.io/en/stable/ and https://pypi.org/
