# GPT Boot Loader

This file explains the sequence used to bootstrap GPTs in the NoteGenLite system.

The following modules are loaded in the order defined in `boot_manifest.json`:

- WorldContext (global context, themes, methodology)
- InteractionCore (reaction rules, tonal, temperature)
- DialogueOrchestration (orchestrated dialog routing flow)
- Personas Amy, Ayase, Ponta

This file should be kept close to `boot_manifest.json` and not loaded directly.

The pathnames in the manifest must be valid GitHub repo paths that can be delivered over RAW.

Make sure to use valid URL encoding when referring to them in GDPTs or external schema declarations.
