# Hogwarts Legacy — Magic Item System

A small Java object model of a Hogwarts Legacy-inspired magic system: wizards cast spells, drink potions, and trade magic items.

## Structure

- **`Wizard`** — casts spells, drinks potions, trades items; has HP, MP, and a magic level
- **`Spell`** (abstract) — `AttackingSpell`, `HealingSpell`, `ProtectingSpell`
- **`MagicItem`** (abstract) — tradeable, magic-capable items
  - **`Potion`** (abstract) — `HealthPotion`, `ManaPotion`, `Concoction`
  - **`Scroll`** — casts a contained spell on its own
- **`MagicLevel`** (enum) — `NOOB`, `ADEPT`, `STUDENT`, `EXPERT`, `MASTER`
- Interfaces: `Tradeable`, `Trader`, `MagicSource`, `MagicEffectRealization`

Requires Java 17+.
