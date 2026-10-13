# Project Card

A project card is a one-page, standardized summary of a project's design and data.
It exists so anyone — a new lab member, a collaborator, a reviewer, or future-you — can learn the essentials of a project without digging through code, chat history, or someone's memory.

This is the same idea as a "model card" or "system card" used elsewhere in ML/AI, applied to a biomedical imaging project: the same sections appear every time, in the same order, so readers always know where to look.

## 1. When to create one

Create a project card when a project starts (even before any data exists — fill in what you know and update it as the project develops), for:

- Any new analysis or data repository (see [GitHub Strategy](github_strategy.md)).
- Any project involving patient/subject samples, a specific cell type, or microscopy imaging.

Skip it only for small, short-lived exploratory work that will not become its own repository.

## 2. How to use it

1. Copy the template at [`templates/project_card_template.md`](templates/project_card_template.md) into the root of the project repository as `PROJECT_CARD.md`.
1. Fill in every section. If a section does not apply, write "N/A" with a one-line reason rather than deleting it — this keeps the same sections present across every project, so readers can rely on their existence.
1. Link `PROJECT_CARD.md` from the project's `README.md`.
1. Keep it up to date: update the card (and its changelog section) whenever the design, data location, or status changes meaningfully, not just at project kickoff.

## 3. What's always included

Regardless of project specifics, every project card answers the same questions:

| Section             | Always answers                                                                |
| ------------------- | ----------------------------------------------------------------------------- |
| Overview            | What is this project, who owns it, what is its status right now?              |
| Design              | What is the hypothesis, the experimental design, and the scale of the data?   |
| Biological material | Who/what are the patients or subjects, and what cell type(s) are used?        |
| Assay               | What stains, dyes, or antibodies mark what, on what channel?                  |
| Imaging             | What microscope, image format, bit depth, and dimensions produced the images? |
| Data                | Where do the raw and processed data live, and who/what can access them?       |
| Contacts            | Who is the PI, project lead, and who else is involved?                        |
| Changelog           | What has materially changed about the project, and when?                      |

See the [template](templates/project_card_template.md) for the full field-by-field layout, including examples (e.g. Cell Painting channel naming) for the assay and imaging sections.

## 4. Why a fixed template

A fixed set of sections (rather than free-form notes) means:

- Readers never have to search for where a particular fact lives — it's always in the same section.
- Missing information is obvious (an empty table cell or an unexplained "N/A"), rather than silently absent from a prose summary.
- Cards are comparable across projects, which matters once the lab runs more than a handful of them at once.
