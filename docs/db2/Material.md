---
sidebar_position: 1
---

# Material

This table defines material types used by items and equipment in the game. It controls armor sound types, sheathing sounds, and more.

---

### Layout:

| ID | Flags | FoleySoundID | SheatheSoundID | UnsheatheSoundID |
|---|---|---|---|---|
| 1 | 1 | 0 | 698 | 700 |
| 2 | 0 | 0 | 697 | 699 |
| 3 | 0 | 0 | 696 | 701 |
| 4 | 1 | 0 | 0 | 0 |
| 5 | 5 | 1005 | 0 | 0 |
| 6 | 3 | 1004 | 696 | 701 |
| 7 | 0 | 0 | 11597 | 11598 |
| 8 | 0 | 1003 | 0 | 0 |


### Hotfix Layout:
No hotfix layout for this DB2

---

### Columns:

- **ID**: Unique identifier for the material entry.
- **Flags**: Bitfield controlling material behavior (e.g., armor type, destructibility).
- **FoleySoundID**: Sound played when armor moves.
- **SheatheSoundID**: Sound when weapon is sheathed.
- **UnsheatheSoundID**: Sound when weapon is unsheathed.

---

### Known Sound References

| Sound ID | Name |
|----------|------|
| 696 | Weapon_Sheathe_Cloth |
| 697 | Weapon_Sheathe_Leather |
| 698 | Weapon_Sheathe_Metal |
| 699 | Weapon_Unsheathe_Leather |
| 700 | Weapon_Unsheathe_Metal |
| 701 | Weapon_Unsheathe_Cloth |
| 1003 | Armor_Foley_Metal_Heavy |
| 1004 | Armor_Foley_Chain |
| 1005 | Armor_Foley_Plate |
| 11597 | Weapon_Sheathe_Fist |
| 11598 | Weapon_Unsheathe_Fist |

You can cross-check these in `SoundEntries.db2` or in `SoundKit.db2` depending on client build.

---

### ID Breakdown

The `ID` column to material Name:

| ID | Material | Comment |
|-----|-------|---------|
| 0 | Consumables | Food, reagents, etc... |
| 1 | Metal |  |
| 2 | Wood | |
| 3 | Miscellaneous | No idea what this could be, its used for caches. |
| 4 | Jewelry |  |
| 5 | Chain |  |
| 6 | Plate |  |
| 7 | Cloth |  |
| 8 | Leather |  |

---


### Flags Breakdown

The `Flags` column is a bitfield:

| Bit | Value | Meaning |
|-----|-------|---------|
| 0 | `0x1` | Hard material type (metal, stone) |
| 1 | `0x2` | Cloth or soft armor |
| 2 | `0x4` | May override default foley sound |
| ... | ... | More bits TBD as they are discovered |

---



### Related Tables


---