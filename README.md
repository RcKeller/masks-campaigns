# Masks: Campaigns

Private campaign content for **Masks: A New Generation** FoundryVTT module.

**This module is not published.** It contains campaign-specific journals, scenes, and NPCs.

## Requirements

- FoundryVTT v13+
- PbtA system v1.1.16+
- [Masks: A New Generation (Unofficial)](https://github.com/RcKeller/masks-newgeneration-unofficial) module

## Contents

### Dispatch Campaign
- `dispatch-journals` - Campaign rules, session recaps, house rules
- `dispatch-scenes` - City locations, HQ maps

## Development

```bash
# Install dependencies
npm install

# Convert JSON to LevelDB (after git pull)
npm run pullJSONtoLDB

# Convert LevelDB to JSON (for version control)
npm run pushLDBtoJSON
```

**Important:** Close Foundry before running pack conversion commands.

## Organization

Packs are prefixed with campaign names:
- `dispatch-*` - Current campaign (Dispatch)
- Future campaigns can add their own prefixes

## License

MIT
