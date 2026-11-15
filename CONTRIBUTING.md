# Contributing to Python Junction

Thank you for helping improve Python Junction. Contributions should make the repository more accurate, understandable and useful to learners.

## Ways to contribute

- Fix incorrect explanations or code.
- Improve clarity, grammar or examples.
- Add exercises with verified solutions.
- Add useful Mermaid diagrams.
- Suggest practical projects.
- Report broken links or outdated information.

## Content standards

1. Explain concepts in clear, professional English.
2. Assume the reader may be new to programming.
3. Use Python 3 and state version-specific requirements when relevant.
4. Keep examples small, focused and runnable.
5. Include expected output where it improves understanding.
6. Explain non-obvious code; do not add unexplained code dumps.
7. Never include passwords, tokens, private keys or personal information.
8. Prefer the Python standard library unless an external dependency is necessary.
9. Link to official documentation for language and library behaviour.
10. Use diagrams only when they clarify a process or relationship.

## Python code style

- Follow [PEP 8](https://peps.python.org/pep-0008/) as the general style guide.
- Use descriptive names such as `calculate_total`, not unclear abbreviations.
- Use four spaces for indentation.
- Keep examples focused on the topic being taught.
- Include comments to explain intent, not to restate every line.

## Suggested workflow

```bash
git clone https://github.com/<your-github-username>/Python_Junction.git
cd Python_Junction
git checkout -b docs/improve-topic-name
```

Make and test your changes, then review them:

```bash
git status
git diff
```

Commit with a clear message:

```bash
git add .
git commit -m "docs: improve Python topic explanation"
git push -u origin docs/improve-topic-name
```

Open a pull request describing:

- What changed.
- Why the change is useful.
- How code examples were tested.
- Any Python version or dependency requirements.

## Before submitting

- [ ] Markdown headings and links render correctly.
- [ ] Code blocks use the correct language identifier.
- [ ] Python examples run successfully.
- [ ] Expected output matches actual output.
- [ ] No secrets or private data are included.
- [ ] The change follows the existing folder and naming conventions.
