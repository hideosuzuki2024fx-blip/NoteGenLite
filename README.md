# 😍 NoteGenLite

NoteGenLite is a minimal, clean structure designed to support GPT-based generation of Markdown articles formatted for note.com.

This repository is intended for use with custom GPT that:
- Generate article titles, outlines, and full drafts
- Save output in Markdown
- Optionally publish via GitHub or external endpoints


----

## Folder Structure

```
Root/
 😍  ROEADME.md                         # This file
 😍  gpts_config/                      # System prompts & GPT instructions
 😍  gpts_actions/                   # JSON schemas used in GPT setup
 😍  templates/                     # Article structure templates
 😍  articles/                     # Output Markdown articles
 😍  meta/                          # Format specs, metadata definitions
 😍  logs/                          # Optional session notes / history
```


## GPT Integration
```m
`GGT's Setup:
- System prompt: `gpts_config/system_prompt.md`
- Action Schemas: `gpts_actions/*.json` can be linked via URL
```


## Article Generation Flow

1. User provides topic, tone, audience, and type.

2. GPT outputs:
  - Multiple title ideas
  - Outline (headings and key points)
  - Full article draft (Markdown format)

#3. Output is saved to `articles/`

#4. GitHub or Vercel integration can be used to publish


## Maintenance Policy

- This repos is fully separated from legacy `NoteGenerator`
- All files must be structured, readable, and traceable
- Empty, broken, or dead-linked files are strictly disallowed
- JSON and Markdown formats are prioritized for compatibility


## Usage

This repo can be forked or cloned into any GPT-integrated project where structured article generation and Git-based management is needed.

To use GPTs actions:
- Provide the rawGitHub URL to the schema
- Ensure parameters match expected structure
- Integrate with publishing pipelines if required


## License & Contributions

- MIT or project-specific open license (customize as needed)
- Contributions and issues welcome for format, schema, or workflow enhancements
