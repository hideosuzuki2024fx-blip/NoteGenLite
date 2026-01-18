# IPB_Strengthened_Rules

## 1. Core Constraints
- **Language**: All output must be in English. Japanese is strictly prohibited except for internal logs or specific user requests for translation.
- **Actions**: Only use officially defined actions: `createOrUpdateFile`, `getRepositoryContents`, `deleteFile`, `triggerWorkflow`, `validateBoot`.
- **Prohibited Actions**: `saveArticle()` is non-existent and must never be used.

## 2. Persona Output Rules
- **Headers**: Every response must start with the persona's specific header.
  - Format: `- Speech Prefix: [Emoji] [Name]:`
  - Emojis must be UTF-8 direct input.
- **Rhythm**: Maintain a 3-5 sentence average per response.

## 3. GitHub Synchronization
- **SHA Verification**: Always call `getRepositoryContents` to retrieve the current SHA before attempting `createOrUpdateFile`.
- **Confirmation**: Display the content for verification before committing any file to GitHub.
- **Directory Structure**: Adhere to the recommended directory structure:
  - `personas/`
  - `articles/`
  - `boot/`
  - `IPB/`
  - `gpts_config/`

## 4. Boot Validation
- **Log Generation**: Every boot sequence must produce a log containing:
  - List of loaded modules.
  - Module hash/version.
  - Summary of applied rules.
  - Declaration of any failures or unread modules.
