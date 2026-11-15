# 🔢 Guess The Number

A terminal Number Guessing Game, built as the day 12 project of Udemy's *100 Days of Code™: The Complete Python Pro Bootcamp*.

## 📚 Table of Contents

- [Overview](#-overview)
- [Requirements](#-requirements)
- [Setup](#-setup)
- [Run](#-run)
- [Tests](#-tests)
- [License](#-license)
- [Links](#-links)
- [Appendix: Project documents](#-appendix-project-documents)

## 🧭 Overview

The computer picks a number between 1 and 100. Choose a difficulty and guess it:

| Level | Attempts |
|-------|----------|
| easy  | 10       |
| hard  | 5        |

After each guess you are told whether it was too high or too low.

### Project layout

```
src/guess_the_number/   game code (constants.py, game.py)
tests/                  pytest tests
docs/                   Doxyfile
```

The functions `set_difficulty`, `check_answer` and `play_game` follow the
course assignment's naming.

### Documentation

Source comments use Doxygen. With [Doxygen](https://www.doxygen.nl/) installed:

```bash
doxygen docs/Doxyfile
```

The HTML output is written to `docs/build/html`.

## 📋 Requirements

- Python 3.13 or newer
- No runtime dependencies (`pytest` is only needed for the tests)

## 🛠️ Setup

Create and activate a local virtual environment, then upgrade pip.

Windows (PowerShell):

```powershell
python -m venv .venv
.venv\Scripts\Activate.ps1
python -m pip install --upgrade pip
```

Linux / macOS:

```bash
python -m venv .venv
source .venv/bin/activate
python -m pip install --upgrade pip
```

## ▶️ Run

```bash
python -m pip install -e .
python -m guess_the_number
```

## 🧪 Tests

```bash
python -m pip install -e ".[dev]"
python -m pytest
```

## 📄 License

See [LICENSE][license].

## 🔗 Links

- [Repository][repository]
- [Documentation][documentation]
- [Issue tracker][issues]

## 📎 Appendix: Project documents

The documents a newcomer needs, in reading order.

| Document | What it tells you |
| --- | --- |
| [Business Case][BC-001] | Why the project exists, its scope and success criteria |
| [Stakeholder Analysis][SA-001] | Who is involved; the stakeholder IDs used for owners and reviewers |
| [Project Plan][PP-001] | The gateways and their schedule |
| [Milestones][milestones] | One document per gateway: Go/No-Go criteria and tasks |
| [Artifact registry][registry] | Where each artifact type lives, the next version, the PO language and domain |
| [Traceability matrix][TM-001] | How the artifacts link and when each was last reviewed |

---

[repository]: https://git.tirsystem.com/Tirsvad-Udemy-100-days-of-code/012-guess-the-number
[documentation]: https://git.tirsystem.com/Tirsvad-Udemy-100-days-of-code/012-guess-the-number/wiki
[issues]: https://git.tirsystem.com/Tirsvad-Udemy-100-days-of-code/012-guess-the-number/issues
[license]: ./LICENSE
[BC-001]: ./docs/business-case.md
[SA-001]: ./docs/stakeholder-analysis.md
[PP-001]: ./docs/project-plan.md
[milestones]: ./docs/milestones/
[registry]: ./docs/artifact-registry.md
[TM-001]: ./docs/sqa/traceability-matrix.md
