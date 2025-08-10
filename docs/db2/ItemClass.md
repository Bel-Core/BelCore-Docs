---
sidebar_position: 1
---

# ItemClass
Here you will be able to learn more about the DB2.


### Layout:

| ID  | ClassNamelang          | ClassID | PriceModifier  | Flags |
|-----|------------------------|---------|----------------|-------|
| 1   | Consumable             | 0       | 0.25           | 0     |
| 2   | Container              | 1       | 0.25           | 0     |
| 3   | Weapon                 | 2       | 0.2            | 1     |
| 4   | Gem                    | 3       | 0.25           | 0     |
| 5   | Armor                  | 4       | 0.2            | 0     |
| 6   | Reagent                | 5       | 0.25           | 0     |
| 7   | Projectile             | 6       | 0.25           | 0     |
| 8   | Tradeskill             | 7       | 0.25           | 0     |
| 9   | Item Enhancement       | 8       | 0.25           | 0     |
| 10  | Recipe                 | 9       | 0.25           | 0     |
| 11  | Money (OBSOLETE)       | 10      | 0.25           | 0     |
| 12  | Quiver                 | 11      | 0.25           | 0     |
| 13  | Quest                  | 12      | 0.25           | 0     |
| 14  | Key                    | 13      | 0.25           | 0     |
| 15  | Permanent (OBSOLETE)   | 14      | 0.25           | 0     |
| 16  | Miscellaneous          | 15      | 0.25           | 0     |
| 17  | Glyph                  | 16      | 0.25           | 0     |
| 18  | Battle Pets            | 17      | 0.25           | 0     |
| 19  | WoW Token              | 18      | 0.25           | 0     |
| 145 | Profession             | 19      | 0              | 0     |


### Hotfix Layout:
| Field | Type | Length | Unsigned | Key | Null | Default | ZeroFill | Extra | Comment |
|-------|------|--------|------------|-----|------|---------|----------|-------|---------|
| ID | INT |  | YES | PRI | NO | 0 | NO |  |  |
| ClassName | TEXT | 65535 | NO |  | YES |  | NO |  |  |
| ClassID | TINYINT |  | NO |  | NO | 0 | NO |  |  |
| PriceModifier | FLOAT |  | NO |  | NO | 0 | NO |  |  |
| Flags | TINYINT |  | YES |  | NO | 0 | NO |  |  |
| VerifiedBuild | INT |  | NO |  | NO | 0 | NO |  |  |


### Columns:

- **ID**: Unique identifier for the ItemClass entry.
- **ClassNamelang/ClassName**: The class name
- **ClassID**: Class ID for usage in other files + tables.
- **PriceModifier**: Price modifier based on the ItemClass.
- **Flags**: NOT KNOWN YET
- **VerifiedBuild**: [See VerifiedBuild ->](/docs/references/VerifiedBuild)

---


### ID Breakdown

The `ID` is not used for anything.

---

### ClassNamelang/ClassName Breakdown

`ClassNamelang/ClassName` is for the class name.

---

### ClassID Breakdown

`ClassID` is the ID used across other files + tables as the identifier for the ItemClass.

---

### PriceModifier Breakdown

`PriceModifier` is the modifier for the price for this ItemClass.
So if its a `Weapon`, it would of course sell for more than a Consumable.

---


### Flags Breakdown

No idea yet, will update when we figure it out.

---

### VerifiedBuild Breakdown

Click "Learn More" to learn about the VerifiedBuild field:
[Learn More →](/docs/references/VerifiedBuild)

---



### Related Tables

None for now.

---



















































<div style={{ fontSize: '0.9em', color: 'var(--ifm-color-content-secondary)' }}>

### 🖋️ Credits

This documentation was written and maintained by [**Sylian**](https://github.com/Sylian1337), creator of **SylCore** and educator on [YouTube](https://www.youtube.com/@DEVSylian).

If you use this, consider contributing back, or showing your support to the authors 🙏

</div>