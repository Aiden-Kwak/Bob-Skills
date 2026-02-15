# Skills

Skills are modular knowledge packages that extend your capabilities for
specific domains or tasks. Think of them as expert onboarding documents:
they contain procedural knowledge, workflows, and resources that you
wouldn't otherwise have.

Skills that you can use are located in the `.bob/skills/` directory.

## When to Use a Skill

Check the skill descriptions in your context.
Use a skill when the user's request clearly matches what the description says to trigger on.

Example description:
GitHub CLI pull request operations using `gh pr`. Use when creating PRs,
listing/viewing PRs, conducting code review workflows, merging PRs,
or managing PR state.

User says: "Can you make a PR for this branch?" -> Trigger this skill

## How to Use a Skill

1. Read `SKILL.md` first - Use `view` to read the skill's main file. This is the routing layer.
2. Follow its routing - `SKILL.md` may point you to reference files for specific tasks.
3. Load references selectively - Only read the reference file you actually need to complete the task.
4. Execute the guidance - Follow the documented commands, patterns, or workflows exactly.

## Progressive Loading Rule (Important)

- Do NOT load all skills or all references.
- Use the short descriptions below to decide which skill is relevant.
- Only open a skill's `SKILL.md` when the request clearly matches.
- Only open `references/` when `SKILL.md` explicitly routes you there.

This rule exists to preserve context and avoid unnecessary loading.

## What NOT to Do

- Don't load everything - only read reference files when you need them.
- Don't ignore skills - they exist because the knowledge is not obvious.
- Don't skip `SKILL.md` - it provides context and routing that references alone lack.

## Skill Structure (General)

Each skill is a folder under `.bob/skills/<skill-name>/`.

At minimum, every skill should provide:
- `SKILL.md` (routing + instructions)

Other subfolders may vary by skill, for example:
- `templates/` (templates or reusable artifacts)
- `scripts/` (executable helpers)
- `assets/` or other resource folders (fonts, images, examples, etc.)

Always follow `SKILL.md` as the routing layer:
- Read `SKILL.md` first
- Then open only the specific files it points to (templates/scripts/resources) as needed


## Available Skills

Design & Creative

- algorithmic-art
  Use when creating generative or algorithmic art using code (e.g. p5.js),
  including flow fields, particle systems, seeded randomness, or computational aesthetics.

- canvas-design
  Use for visual layout, canvas-based design, and spatial composition tasks.

- frontend-design
  Use for UI/UX design guidance, frontend layout decisions, and interface patterns.

- theme-factory
  Use when creating or adapting reusable themes, design systems, or visual styles.

Documents & Files

- pdf
  Use for reading, summarizing, extracting, or generating PDF documents.

- docx
  Use for Microsoft Word (.docx) workflows: drafting, editing, restructuring documents.

- pptx
  Use for creating or editing slide decks and presentation materials.

- xlsx
  Use for spreadsheet workflows: transforming data, translating tables, formatting, or exporting Excel files.

- doc-coauthoring
  Use for collaborative writing workflows and structured document co-authoring.

Web & Artifacts

- web-artifacts-builder
  Use when producing web-ready deliverables or artifacts from content or data.

- webapp-testing
  Use for planning, designing, or executing web application testing workflows.

Communication

- internal-comms
  Use for internal announcements, stakeholder communication, and structured messaging.

- slack-gif-creator
  Use when creating Slack-friendly GIFs or short visual assets for communication.

Skills Tooling & Meta

- skill-creator
  Use to create new skills: scaffold folders, generate `SKILL.md`, and set up references.

- template-skill
  Use as a baseline template when creating a new skill package.

- mcp-builder
  Use for MCP-related packaging, tool definitions, and build workflows.
