# viet-style

**English** | [Tiếng Việt](README.vi.md)

A skill for AI assistants that sets the characters, punctuation and layout rules for finished Vietnamese documents. It picks one standard by document type: APA 7 for academic text, Decree 30/2020/NĐ-CP for administrative documents and project files, and a set of general rules for everything else. The skill instructions (`SKILL.md`) are written in Vietnamese.

## What the skill does

- **Chooses one standard by document type** and does not mix them: academic text (APA 7), administrative documents and project files (Decree 30/2020/NĐ-CP), other text (general rules).
- **General rules** (V01 to V04): short hyphen instead of long dashes, curved quotation marks, the word "và" instead of "&", no comma before "và". New rules are added as one table row.
- **Administrative documents and project files:** layout, fonts, margins, document number, place and date, content structure, signature block, recipients, annexes, abbreviations of document types, templates, capitalization, copies. This part is in `references/nghi-dinh-30.md` and is read only when such a document is being drafted.
- **Review before delivery:** the draft is re-read against the chosen standard, and the user is told which standard was applied.

## Boundaries

- Applies to finished Vietnamese documents the user will send or publish, and to text drafted on a canvas or artifact.
- Does **not** apply to ordinary chat answers, code, variable names, commands, commit messages, or English text and verbatim quotations.
- Covers characters, punctuation and layout only. It has nothing on writing style or subject-matter method.

## Folder structure

```
viet-style/
  SKILL.md
  references/
    nghi-dinh-30.md   # Decree 30/2020/NĐ-CP: layout, templates, capitalization
README.md
README.vi.md
LICENSE.md
```

## Installation

### Claude apps (claude.ai, Claude desktop)

1. Download the repo and zip the `viet-style` folder as `viet-style.zip` (the zip must contain the `viet-style` folder at its top level, with `SKILL.md` and `references/` inside).
2. Open Claude, go to **Customize → Skills**, click **+** → **Create skill** → **Upload a skill**, and choose `viet-style.zip`. Menu names and locations may differ between app versions. Skills require code execution to be enabled.
3. Check that the `viet-style` skill is listed and turned on.

### Claude Code

Copy the `viet-style` folder into `~/.claude/skills/` (available in all projects) or into a project's `.claude/skills/`, then restart Claude Code.

## Usage

The skill triggers when you draft, edit, review or convert a finished Vietnamese document, with or without a command. Examples:

- "Draft an official letter to the Department of Planning and Investment about …"
- "Check this project description against Decree 30 layout."

## Limits

- The Decree 30 part was checked against an OCR reading of the scanned original. The positions of the layout boxes, the two default margin and font sets, and the handling of project descriptions are inferred from diagrams, templates or practice, not from the decree's own wording.
- Annexes IV to VI of the decree (registers, management systems) are not included.
- For APA 7 applied to Vietnamese authors and titles, follow the official APA guidance or the rules of the school or journal.
- Review is done by re-reading the text, not by a script.

## Feedback

Please use the repo's **Issues**. It helps to include: the document type, the standard you expected, and the result you got (personal or confidential information removed).

## License

Released under **CC BY-NC 4.0**: free for non-commercial use with attribution. For commercial use, contact the author via **Issues**. See [LICENSE.md](LICENSE.md).
