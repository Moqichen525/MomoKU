# Character Presence

[中文说明](README.md) | English

A Chinese-language skill for GPT Image character generation, controlled image editing, expressive portraits, character design, and consistent multi-view reference assets.

## What it does

- **Character generation:** turn a character brief into visible appearance, expression, action, and scene details.
- **Targeted edits:** change only the requested elements while preserving identity, clothing layers, trousers, footwear, accessories, and the background.
- **Expressions and characterization:** portray attitudes such as deference, condescension, or restrained anger without redesigning the character's face.
- **Multi-view and video references:** maintain a shared identity baseline, wardrobe versions, left/right details, and continuity between shots.

## Package contents

```text
character-presence/
├── SKILL.md
├── README.md
├── README.en.md
└── references/
    ├── continuity.md
    ├── examples.md
    └── personality.md
```

[SKILL.md](SKILL.md) is the entry point. Keep the entire folder intact: supporting documents are loaded through relative links when relevant.

The skill instructions and reference documents are in Chinese. This English guide explains installation and use; it is not a separate English translation of the full skill. You can request English prompts and responses explicitly.

## Installation

Give the following request to an assistant that supports installing skills from GitHub:

> Install the skill at https://github.com/Moqichen525/MomoKU/tree/main/skills/character-presence.

Installation and skill discovery depend on the host application. Downloading the files or opening this README alone does not install the skill. Keep any existing installation backed up before replacing it.

## Usage examples

Once the skill is installed and loaded, use `$character-presence` in hosts that support explicit skill invocation.

### Generate reference views

> Use $character-presence to create front, left-side, and back reference views of the attached character. Keep the face, hairstyle, body proportions, clothing, and footwear consistent. Provide the accompanying notes in English.

### Edit only specified details

> Use $character-presence to remove the beard and black undershirt only. Keep the original long trousers, black shoes, robe, background, and all reference-view layouts unchanged.

### Write prompts without generating images

> Use $character-presence to write two English prompts showing contrasting attitudes for this fictional status-conscious character: eager to please an influential person, and dismissive toward someone they do not wish to help. Keep the same face and outfit. Return prompts only; do not generate images.

### Change an expression

> Use $character-presence to change only the character's neutral expression to restrained anger. Preserve facial structure, age, hairstyle, clothing, camera angle, and lighting. Do not add props or other people.

## Requirements and limitations

This is an instruction package, not a model, API key, or standalone image generator. Prompt writing does not require an image tool. Actual generation and editing require an appropriate tool and access in the host application. Loading this skill does not automatically generate images.

Character traits are supplied as fictional design intentions. Traditional visual conventions may inform styling, but the skill does not infer a real person's morality or personality from facial appearance.

Consistency must be checked in actual outputs. A multi-view sheet helps review a character but is not automatically a suitable first frame for a video. Video continuity requires testing in the chosen video model and reviewing the resulting footage; the skill cannot guarantee identical identity or error-free continuity.

## Validation status

Packaged on October 21, 2026. The package has passed SKILL.md structural validation, relative-link checks, and a content check. Files uploaded to GitHub are read back and compared with the local package.

Packaging does not constitute a new image-quality, video-continuity, or installation-discovery test. Source links are included in the skill and its reference documents. The package excludes character photographs, local machine paths, maintenance logs, credentials, test dependencies, and backups.

