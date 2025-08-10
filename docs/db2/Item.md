---
sidebar_position: 1
---

# Item

### File Layout:
Below is the Item.db2, please note, this is not the full file dumped, but the File Layout is the most important.

<details>
<summary>See Layout</summary>
| ID | ClassID | SubclassID | Material | InventoryType | SheatheType | Sound_override_subclassID | IconFileDataID | ItemGroupSoundsID | ContentTuningID | ModifiedCraftingReagentItemID | CraftingQualityID |
|---|---|---|---|---|---|---|---|---|---|---|---|
| 17 | 4 | 4 | 6 | 4 | 3 | -1 | 132759 | 11 | 0 | 0 | 0 |
| 25 | 2 | 7 | 1 | 21 | 3 | -1 | 135274 | 8 | 0 | 0 | 0 |
| 35 | 2 | 10 | 2 | 17 | 2 | -1 | 135145 | 13 | 0 | 0 | 0 |
| 36 | 2 | 4 | 2 | 21 | 3 | -1 | 133478 | 8 | 0 | 0 | 0 |
| 37 | 2 | 0 | 1 | 13 | 3 | -1 | 132402 | 8 | 0 | 0 | 0 |
| 38 | 4 | 0 | 7 | 4 | 0 | -1 | 135009 | 7 | 0 | 0 | 0 |
</details>

### Hotfix Layout:
<details>
<summary>See Layout</summary>
| Field | Type | Length | Unsigned | Key | Null | Default | ZeroFill | Extra | Comment |
|-------|------|--------|------------|-----|------|---------|----------|-------|---------|
| ID | INT |  | YES | PRI | NO | 0 | NO |  |  |
| ClassID | TINYINT |  | YES |  | NO | 0 | NO |  |  |
| SubclassID | TINYINT |  | YES |  | NO | 0 | NO |  |  |
| Material | TINYINT |  | YES |  | NO | 0 | NO |  |  |
| InventoryType | TINYINT |  | NO |  | NO | 0 | NO |  |  |
| SheatheType | TINYINT |  | YES |  | NO | 0 | NO |  |  |
| SoundOverrideSubclassID | TINYINT |  | NO |  | NO | 0 | NO |  |  |
| IconFileDataID | INT |  | NO |  | NO | 0 | NO |  |  |
| ItemGroupSoundsID | TINYINT |  | YES |  | NO | 0 | NO |  |  |
| ContentTuningID | INT |  | NO |  | NO | 0 | NO |  |  |
| ModifiedCraftingReagentItemID | INT |  | NO |  | NO | 0 | NO |  |  |
| CraftingQualityID | INT |  | NO |  | NO | 0 | NO |  |  |
| VerifiedBuild | INT |  | NO |  | NO | 0 | NO |  |  |
</details>


### Columns:

- **ID**: Unique identifier for the item entry.
- **ClassID**: ID for the Class (Weapon, Plate, Leather...) [See ItemClass.db2 →](/docs/db2/ItemClass)
- **SubclassID**: ID for the sub-class (Twohanded, one-handed, chest, robe...) [See ItemSubclass.db2 →](/docs/db2/ItemSubClass)
- **Material**: ID for the item's material type, used for sound and visual logic. [See Material.db2 →](/docs/db2/Material)
- **InventoryType**: Equipment slot the item occupies. [See InventoryType →](/docs/references/InventoryType)
- **SheatheType**: ID of the sheathe type, so location of the weapon when not holding item.
- **SoundOverrideSubclassID**: ID of the sound subclass for overriding the sound (Might need to update later)
- **IconFileDataID**: ID of an icon image used in the client. [See FileDataID →](/docs/references/FileDataID)
- **ItemGroupSoundsID**: ID of the group of sounds this item uses [See ItemGroupSounds.db2 ->](/docs/db2/ItemGroupSounds)
- **ContentTuningID**: NOT KNOWN YET!
- **ModifiedCraftingReagentItemID**: NOT KNOWN YET!
- **CraftingQualityID**: ID of the crafting quality that this item has, crafting qualities are only for reagent items, not crafted items themselves. [See CraftingQuality.db2 ->](/docs/db2/CraftingQuality.md)
- **VerifiedBuild**: [See VerifiedBuild ->](/docs/references/VerifiedBuild)
---

### ClassID Breakdown

Click "Learn More" to learn about the ClassID field:
[Learn More →](/docs/db2/ItemClass)

---

### SubclassID Breakdown

Click "Learn More" to learn about the SubclassID field:
[Learn More →](/docs/db2/ItemSubClass)

---

### Material Breakdown

Click "Learn More" to learn about the Material field:
[Learn More →](/docs/db2/Material)

---

### InventoryType Breakdown

See full list here: [InventoryType Reference →](/docs/references/InventoryType)

---

### SheatheType Breakdown

(Update this)
See full list here: 
[Learn More →](/docs/db2/ItemGroupSounds)

---

### SoundOverrideSubclassID Breakdown

(Update this)
See full list here: 
[Learn More →](/docs/db2/ItemGroupSounds)

---

### IconFileDataID Breakdown

Click "Learn More" to learn about the IconFileDataID field:
[Learn more](/docs/references/FileDataID)

---

### ItemGroupSounds Breakdown

See full list here: 
[Learn More →](/docs/db2/ItemGroupSounds)

---

### ContentTuningID Breakdown

(Update this)
See full list here: 
[Learn More →](/docs/db2/ItemGroupSounds)

---

### ModifiedCraftingReagentItemID Breakdown

(Update this)
See full list here: 
[Learn More →](/docs/db2/ItemGroupSounds)

---

### CraftingQualityID Breakdown

Click "Learn More" to learn about the CraftingQualityID field:
[Learn More →](/docs/db2/CraftingQuality.md)

---

### VerifiedBuild Breakdown

Click "Learn More" to learn about the VerifiedBuild field:
[Learn More →](/docs/references/VerifiedBuild)

---




















<div style={{ fontSize: '0.9em', color: 'var(--ifm-color-content-secondary)' }}>

### 🖋️ Credits

This documentation was written and maintained by [**Sylian**](https://github.com/Sylian1337), creator of **SylCore** and educator on [YouTube](https://www.youtube.com/@DEVSylian).

If you use this, consider contributing back, or showing your support to the authors 🙏

</div>