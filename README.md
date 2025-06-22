# ChefKnight Encyclopedia

This repository contains the content for the ChefKnight wiki/encyclopedia system. It is designed to work with the [ChefKnight platform](https://github.com/JoshuaHoare/ChefKnight) but can also be used independently as a standalone lore repository.

## 📁 Directory Structure

- `kingdoms/` - Top-level political entities (nations, empires, realms)
- `characters/` - Characters from the story universe
- `regions/` - Geographic areas (provinces, forests, seas)
- `continents/` - Large landmasses spanning multiple regions
- `races/` - Sapient species or ethnic groups
- `foods/` - Cuisine, dishes, ingredients, and recipes
- `abilities/` - Magical powers, special abilities, and skills
- `weapons/` - Armaments, weapons, and offensive tools
- `armour/` - Protective gear and defensive equipment
- `items/` - Artifacts, key objects not covered above
- `religion/` - Deities, belief systems, and religious practices
- `assets/` - Images and other binary files (managed by Git LFS)

## 📝 Content Format

All content is stored as Markdown files with YAML front matter metadata. This format allows for rich text content while maintaining structured data that can be easily parsed by the ChefKnight platform.

### Example: Kingdom Entry

```markdown
---
name: Aldoria
type: Kingdom
region: Northern Realms
ruler: King Thalion IV
population: 3.5 million
climate: Temperate
founded: 892 CR
status: Active
---

# Kingdom of Aldoria

Aldoria is one of the oldest human kingdoms in the Northern Realms...

## Geography

Aldoria spans the fertile plains between the Azure Mountains...

## Government

The kingdom is ruled by King Thalion IV of House Valorian...
```

### Example: Character Entry

```markdown
---
name: Chef Brandish
title: Royal Culinary Knight
kingdom: Aldoria
race: Human
specialties:
  - Battle Cooking
  - Fire Cuisine
  - Defensive Pastry
signature_dish: Flambé Fortress Soufflé
weapon: Whisk Blade
status: Active
---

# Chef Brandish

Chef Brandish is one of the most renowned Culinary Knights...

## Background

Born to a humble baker in the outskirts of Highcrown...
```

## 🖼️ Binary Files

Binary files such as images are stored in the `assets/` directory and are managed using Git LFS (Large File Storage) to keep repository size manageable. Reference these assets in your Markdown content like this:

```markdown
![Chef Brandish](/assets/characters/chef_brandish.jpg)
```

## 📊 Cross-References and Metadata

Use YAML front matter to establish connections between content. For example, characters can reference their home kingdom, items can reference their creator, etc.

## 🤝 Contributing

1. Clone this repository
2. Create new content following the established format
3. Submit a pull request with your additions

## 🔄 Integration with ChefKnight Platform

This content repository is designed to be used as a subrepo within the main ChefKnight application, which provides a web interface for viewing and editing content. See the [ChefKnight repository](https://github.com/JoshuaHoare/ChefKnight) for setup instructions.
