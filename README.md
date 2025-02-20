# Automated Resume Generator

This repository contains my resume in multiple languages with automatic PDF generation using GitHub Actions.

## Features

- Markdown-based resume writing
- Automatic PDF generation on updates
- Multi-language support
- Clean, version-controlled resume management

## How It Works

When changes are pushed to any `resume_*.md` file in the main branch, GitHub Actions automatically:

1. Sets up a Pandoc environment
2. Converts the modified Markdown files to PDF
3. Commits and pushes the generated PDFs back to the repository

## File Structure 
.
├── resume_eng_v1.md     # English version of resume
├── resume_eng_v1.pdf    # Auto-generated English PDF
├── resume_ger_v1.md     # German version of resume
├── resume_ger_v1.pdf    # Auto-generated German PDF
└── .github/
    └── workflows/
        └── convert-resume.yml  # GitHub Actions workflow

## Usage

1. Create your resume in markdown format following the naming convention:
   - `resume_[language]_v[number].md`
   - Example: `resume_eng_v1.md`, `resume_ger_v2.md`

2. Write your resume using standard markdown syntax
   - Use headers (#, ##) for sections
   - Lists for skills and experiences
   - Tables for structured data if needed

3. Commit and push your changes
   - GitHub Actions will automatically generate the PDF version
   - The PDF will be committed back to the repository

## Requirements

The automation uses:
- Pandoc for MD to PDF conversion
- LaTeX for PDF generation
- GitHub Actions for automation

## Contributing

Feel free to fork this repository and adapt it for your own resume management needs.

## License

MIT License - Feel free to use and modify for your own purposes.