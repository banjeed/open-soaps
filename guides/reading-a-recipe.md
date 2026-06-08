# How to read a recipe file

Each recipe in this repository uses a standard format.

---

## YAML front matter

At the top of every recipe is a YAML block (between `---` markers) containing metadata:

```yaml
---
title: "Recipe name"
version: "1.0"
scent_family: citrus
base_oil: olive
secondary_oils: [coconut, castor]
superfat: 5
water_ratio: 38
batch_size_g: 500
cure_weeks: 6
contributed_by: "@username"
date: 2024-01-15
---
```

**`base_oil`** — The dominant oil (by weight %). This is the primary tag used for GitHub search filtering.

**`secondary_oils`** — Supporting oils. Also searchable.

**`scent_family`** — Matches the folder the recipe lives in. One of: floral, citrus, earthy, woody, herbal, unscented.

**`water_ratio`** — Water as a percentage of total oil weight.

**`batch_size_g`** — Total oil weight in grams the recipe is written for. Scale proportionally.

---

## Scaling a recipe

To scale up or down:
1. Change the total oil weight.
2. Re-run the lye amount through a lye calculator using the same oil percentages and superfat.
3. Scale water proportionally.

**Never scale a recipe by changing lye amounts manually** — always recalculate.

---

## Versioning

Recipes use semantic-style versioning:
- `1.0` — original published recipe
- `1.1` — minor tweak (fragrance change, process note)
- `2.0` — significant reformulation (oil percentages changed)

Version history lives at the bottom of each recipe file.
