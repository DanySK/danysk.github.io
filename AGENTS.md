Run `hugo` from the repository root to validate any content or template change before finishing.

When adding or updating a publication entry, keep the existing repository structure:
- Create or edit `content/portfolio/<year-slug>/index.md`.
- Keep front matter aligned with nearby entries: `title`, `date`, `jobDate`, `work`, `designs`, `thumbnail`, and `projectUrl`.
- Store publication-specific assets inside the same `content/portfolio/<year-slug>/` directory and reference them with repository-relative paths already used in the repo.

For new papers, never create or use generated images.
- Use the most appropriate and inspirational image taken from the paper itself.
- Prefer figures, diagrams, or visual material that best represents the contribution of the paper.
- Set `thumbnail` to that sourced image and keep the asset next to the paper entry.
- If you cannot fetch a suitable image from the paper, stop and ask the user instead of inventing, generating, or substituting an unrelated image.

Keep changes narrow and consistent with the existing wording and formatting style of neighboring publication entries.
