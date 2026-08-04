# Contributing

This repository is a free resource for certification practice questions. Contributions are welcome!

## How to Add a New Exam

Since this repo is a public resource for students to practice exams, exam data is added manually through pull requests. Follow these steps:

### 1. Prepare the Exam Data

Create the exam files manually:

- `certifications/<provider>/<exam name>/<level>.md` — Markdown file with practice questions in GFM format
- `data/<slug>/<level>/questions.json` — Structured question data
- `data/<slug>/<level>/metadata.json` — Exam metadata

### 2. Follow the Format

Each exam markdown file must follow the GFM format:

- **Header** with exam name and level
- **Table of Contents** linking to each domain
- **Exam Information** section (7 rows, no URLs to certilum.com)
- **Domain Distribution** table
- **Questions** organized by domain with `<details>`/`<summary>` collapsible sections
- **Task lists** for options (`- [ ]`)
- **Alert syntax** `[!TIP]` for explanations
- **Collapsible answer sections** (answers hidden by default)

### 3. Verify the Output

Check that:
- The markdown file contains the correct number of questions
- Questions are distributed proportionally across all domains
- No URLs to certilum.com or external CTAs are present
- All JSON files are valid and parseable

### 4. Submit a Pull Request

```bash
git add certifications/<provider>/<exam name>/ data/<slug>/
git commit -m "feat: add <exam name> <level> practice questions"
git push
```

Then open a pull request. The repo admin will review and approve your contribution.

## Adding a New Level

To add a new level (e.g., Master, Proficiency) for an existing exam:

1. Create the markdown and JSON files for the new level following the GFM format
2. Place them in the appropriate directory structure
3. Submit a pull request for review

## Reporting Issues

If you find an error in a question or explanation, please open a GitHub issue with:
- The exam name and level
- The question ID
- A description of the error
- Your suggested correction

## Code of Conduct

Be respectful and constructive in all interactions. This is a community resource.

## License

Contributions are licensed under the MIT License.
