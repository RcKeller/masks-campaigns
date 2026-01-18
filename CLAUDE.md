# Masks: Campaigns

Private module for campaign-specific content. NOT published.

## Overview

- **Module ID:** `masks-campaigns`
- **Type:** Campaign content (journals, scenes)
- **Dependency:** Requires `masks-newgeneration-unofficial`
- **Status:** Private (not published)

## Structure

```
masks-campaigns/
├── module.json
├── packs/
│   ├── dispatch-journals/    # LevelDB (gitignored)
│   └── dispatch-scenes/      # LevelDB (gitignored)
├── src/packs/
│   ├── dispatch-journals/    # JSON source (version controlled)
│   └── dispatch-scenes/      # JSON source (version controlled)
├── images/
│   ├── maps/                 # Scene background images
│   └── tokens/               # NPC tokens
├── tools/
└── package.json
```

## Pack Organization

Use campaign prefixes to organize content:
- `dispatch-*` - Dispatch campaign
- Future campaigns would use their own prefix (e.g., `legacy-*`)

## Commands

```bash
npm install              # Install dependencies
npm run pullJSONtoLDB    # JSON → LevelDB (after git pull)
npm run pushLDBtoJSON    # LevelDB → JSON (for version control)
```

**Important:** Foundry must be closed when running pack conversion.

## Adding New Content

1. Create content in Foundry
2. Close Foundry
3. Run `npm run pushLDBtoJSON`
4. Commit the JSON changes

## Image Paths

Maps: `modules/masks-campaigns/images/maps/{filename}`
Tokens: `modules/masks-campaigns/images/tokens/{filename}`
