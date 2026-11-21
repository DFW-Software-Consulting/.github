# Organisation profile repo overview

This is the organisation-level `.github` repository. It holds no application code, build or tests; every file is Markdown or YAML that GitHub reads directly.

## What is in it

- `profile/README.md`: the organisation profile page. GitHub renders it at the top of the organisation's public page. Content: tagline, badges, what we do, how we work, ways to work together, recent work, team, contact details.
- `SECURITY.md`: the org-wide security policy. Repositories without their own policy inherit it. It asks reporters to email privately and not to open public issues.
- `.github/PULL_REQUEST_TEMPLATE.md`: default pull request template (what and why, how tested, linked issue, checklist) for repositories that have none.
- `.github/ISSUE_TEMPLATE/bug_report.yml`, `feature_request.yml`: default issue forms. `config.yml` keeps blank issues enabled and adds a contact link for private security reports.

## How the profile renders

GitHub looks for `profile/README.md` in the organisation's `.github` repository (public) and shows it on the organisation page. Edits merged to the default branch appear without any build step. It is plain GitHub-flavoured Markdown: the badges are image links, and relative links do not work well there, so use absolute URLs.

## Conventions

- Defaults here apply only to repositories that lack their own copy of a file, and the repo must stay public for the profile to show.
- Everything is public. Keep contact details to the ones already published; add no internal hosts, client names beyond the generic "recent work" wording, or credentials.
- History shows the tech stack section was removed from the profile on purpose (commit fd47ad0); do not re-add it without being asked.
- Changes go through pull requests, using the template in this repo.
