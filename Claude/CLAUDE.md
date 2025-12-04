# General Guidelines

- Provide concise responses while making sure that relevant details are not omitted
- Follow SOLID principles

# Source Code-Specific

- Follow the code style of the given module
- When adding executable code into docstrings, use `<code>` (e.g., `enabled=True`)
- For type hints, use abstraction on the input but concrete types on the output, i.e., `def f(arr: Iterable[str]) -> list[int]:` except for unit tests which should always use concrete types
- Do not use `dict` as a type hint, but prefer `dict[str, Any]` if applicable
- Never use relative imports unless necessary
- Prefer importing identifiers directly when they are part of our codebase, but 3rd party modules should be imported as a whole (e.g., `from rir_models.labels import Attribute` and `import more_itertools`)

# Plan Mode

- Make the plan multi-phase provided the changes are complex enough
- At the end of each plan, provide a list of unresolved questions. Make the questions concise and straightforward

# Git

- Prioritize short commit messages but add details to the commit description
- When creating branches, prefix them with "mo/" and use dashes to separate individual words (e.g., "mo/azure-ocr")
- Prefer short commits with minimal diffs that encapsulate a single change focused to a given module
- Find an appropriate GitMoji to describe the commit intent (e.g. "morgan: :sparkles: Implement support for multi-threading")
- Start each commit message with a module name, e.g. "commons: Add support for checkboxes in Azure OCR"
- Make sure that the order of commits is logical and the codebase is always testable after each commit
- When adding docstrings or type hints to existing code, make sure that these changes are made prior to implementing new features and committed separately

# Running Tests

- Use `micromamba activate rir` to activate the Python environment
- Use `pytest --last-failed --maxfail=1 --force-short-summary --disable-warnings --no-header --quiet` to run test
