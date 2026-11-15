# Running Python Scripts

> Part of [Module 01 — Python Environment Setup](../README.md).

Create a file called `hello.py`:

```python
print("Hello from Python Junction!")
```

Run from Ubuntu/WSL:

```bash
python3 hello.py
```

Run from Windows PowerShell:

```powershell
python hello.py
```

Expected output:

```text
Hello from Python Junction!
```

If the file is not in the current directory, provide its correct path. If the command selects the wrong interpreter, inspect `sys.executable`.
