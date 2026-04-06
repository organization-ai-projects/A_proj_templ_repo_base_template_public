# Repo Base Template Public

Public template repository for the base repository.

## Purpose

This repository stores the baseline files used to initialize a new repository.
It is not itself the final generated repository layout.

## Structure

- `repository_elements/`: files and directories copied into the root of the generated repository
- `README.md`: documentation for this template repository
- `.gitignore`: ignore rules for this template repository workspace
- `.markdownlint.json`: Markdown lint configuration for this template repository workspace

## Why `repository_elements/` exists

GitHub treats a root `.github/workflows/` directory as active workflow configuration for the
current repository. The template content therefore lives under `repository_elements/` so that
workflow files, issue templates, and other repository metadata remain inert until copied into a
real target repository.

## Template Contents

`repository_elements/` currently includes:

- repository automation workflows
- issue and pull request templates
- labels configuration
- repository-level Markdown and Git ignore defaults
- a starter `README.md` with placeholders to replace during repository creation

## Generation Rule

When creating a new repository from this template, copy the contents of `repository_elements/`
into the root of the target repository.

## Notes

- Root-level files in this repository apply only to the template repository itself.
- Files inside `repository_elements/` are the ones intended for the generated repository.
