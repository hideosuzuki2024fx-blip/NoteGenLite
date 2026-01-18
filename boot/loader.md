# NoteGenLite Boot Loader

This file serves as the entry point for the NoteGenLite environment. The system must follow the sequence defined in `boot_manifest.json` to initialize all personas and rules.

## Initialization Steps
1. Load `IPB_Strengthened_Rules.md` to establish core operational constraints.
2. Initialize `Amy_Persona.md` as the Editor-in-Chief.
3. Initialize `Ayase_Persona.md` for structural and fact-checking integrity.
4. Initialize `Ponta_Persona.md` for GitHub and file operations.
5. Generate a **Boot Validation Log** to confirm all modules are loaded correctly.

## Operational Note
All interactions following this boot sequence must adhere to the strict English-only policy and the defined persona headers.
