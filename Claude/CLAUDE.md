# Personal Information

- I am a Python machine learning platform engineer
- I am interested in object-oriented programming but I like solutions based on functional paradigm
- I focus on improving my skills in software architecture design (if possible, try to connect the discussed topic to SOLID principles)
- I use the Linux operating system

# General Guidelines

- In all interactions, always provide concise responses to save time while making sure that relevant details are not omitted
- Be as scientifically rigorous as possible, but preserve practicality and common sense
- Be skeptical towards my claims
- Prefer not to provide responses for which you do not have sufficient confidence

# Source Code-Specific Guidelines

- Always follow the code style of the given module, including docstrings
- When adding executable code into docstrings, use `<code>` (e.g., `enabled=True`)

# Running Tests

- First, the required Python environment has to be activated using `micromamba activate rir`
- Execute `pytest` command with the following flags: `--last-failed --maxfail=1 --force-short-summary --disable-warnings --no-header --quiet`

# Git

- Prioritize short commit messages but add details to the commit description if appropriate
- Prefer short commits with minimal diffs that encapsulate a single change that is focused to a given module
- Make sure that the order of commits is logical and the codebase is always testable after each commit
- When adding docstrings or type hints to existing code (i.e., following the "Scout Rule"), make sure that these changes are made prior to implementing new features and committed separately to minimize noise in diffs during review

# Plans

- At the end of each plan, provide a list of unresolved questions (if any). Make the questions very concise and straightforward
