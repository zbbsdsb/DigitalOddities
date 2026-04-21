# GitHub Configuration

This directory contains GitHub-specific configuration files for the DigitalOddities project.

## Directory Structure

```
.github/
├── ISSUE_TEMPLATE/        # Templates for GitHub Issues
│   └── artifact-submission.md  # Template for submitting new artifacts
├── workflows/            # GitHub Actions workflows
│   └── weekly-showcase.yml     # Weekly showcase generation workflow
└── PULL_REQUEST_TEMPLATE.md    # Template for Pull Requests
```

## Files Description

### 1. ISSUE_TEMPLATE/artifact-submission.md

A standardized template for submitting new digital artifacts to the collection. This template guides contributors through the process of providing all necessary information for their artifact, including:

- Theme selection
- Artifact title and ID
- Status and location
- Detailed description
- Visual element (ASCII, emoji, table, etc.)
- Interactive prompt for other contributors

### 2. workflows/weekly-showcase.yml

A GitHub Actions workflow that automates the weekly showcase generation process. This workflow:

- Runs every Sunday at midnight UTC
- Can also be triggered manually
- Calculates the current and next week's theme
- Generates a weekly showcase markdown file
- Updates the current theme in the main README
- Notifies maintainers to review and publish the showcase

### 3. PULL_REQUEST_TEMPLATE.md

A standardized template for submitting Pull Requests with new artifacts. This template includes:

- Artifact details (theme, title, ID, file path)
- Brief description
- Checklist to ensure submission quality

## How to Use These Files

### For Contributors

1. **Submitting an Artifact via Issue**: 
   - Click "New Issue" in the GitHub repository
   - Select the "Artifact Submission" template
   - Fill out all required fields
   - Submit the Issue

2. **Submitting an Artifact via Pull Request**: 
   - Fork the repository
   - Create your artifact in the appropriate theme directory
   - Open a Pull Request
   - The PR template will guide you through the submission process

### For Maintainers

1. **Reviewing Submissions**: 
   - Check Issue submissions for completeness
   - Review PRs against the checklist
   - Merge approved PRs

2. **Managing the Weekly Showcase**: 
   - The workflow will generate the showcase automatically
   - Review the generated showcase at `.github/workflows/temp/showcase.md`
   - Publish the showcase as a Discussion post

## Configuration Notes

- All files follow GitHub's official documentation and best practices
- The weekly showcase workflow uses Python and the PyGithub library
- Templates are designed to be user-friendly and guide contributors through the submission process

For more information on GitHub Actions, Issue templates, and PR templates, please refer to the [GitHub documentation](https://docs.github.com/).
