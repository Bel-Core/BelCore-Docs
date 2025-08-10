

# VerifiedBuild

The `VerifiedBuild` field is used in most hotfix-enabled DB2 tables to determine which client build a row applies to. This value must match the client's internal build number for the row to be loaded.

---

### Purpose

When the WoW client starts, it reads its internal build number (e.g. 54845 for 10.2.7). For each hotfix-enabled DB2, it will only load rows where `VerifiedBuild` matches the client's current build. Any rows with mismatched builds are ignored.

---

### Common Usage

This field appears in nearly every hotfix-enabled DB2 table, including but not limited to:

- `Item.db2`
- `ItemSparse.db2`
- `SpellName.db2`
- `CurrencyTypes.db2`
- `MapDifficulty.db2`
- `QuestV2.db2`
- `ItemModifiedAppearance.db2`
- `ItemDisplayInfo.db2`

It is also used in the `HotfixData` control table that governs hotfix application.

---

### Typical Build Values

| Build    | Patch     | Description                |
|----------|-----------|----------------------------|
| 45342    | 9.2.0     | Shadowlands                |
| 49516    | 10.0.0    | Dragonflight pre-patch     |
| 52689    | 10.1.7    | Dragonflight content patch |
| 53781    | 10.2.5    | Seeds of Renewal           |
| 54845    | 10.2.7    | Final pre-TWW build        |

These values change regularly with retail and PTR builds.

---

### How to Find the Correct Build Number

To ensure your data loads in the client, `VerifiedBuild` must match the current build. You can find the active build number by:

- Reading the `.build.info` file in the WoW client directory
- Inspecting `HotfixData.db2` from a client data dump
- Using tools like [WoW.tools](https://wow.tools/dbc) or [TrinityDBCEditor](https://github.com/KitzBlitzTrinity/TrinityDBCEditor)

---

### Best Practices

- Always provide a valid `VerifiedBuild` when inserting rows into hotfix-enabled tables
- Keep this value updated when moving to new retail builds or patches
- Avoid using placeholder or outdated build numbers, as they will be silently ignored by the client

---

### Related Pages

- [Item.db2](/docs/db2/Item)

---

<div style={{ fontSize: '0.9em', color: 'var(--ifm-color-content-secondary)' }}>

### 🖋️ Credits

This documentation was written and maintained by [**Sylian**](https://github.com/Sylian1337), creator of **SylCore** and educator on [YouTube](https://www.youtube.com/@DEVSylian).

If you use this, consider contributing back, or showing your support to the authors 🙏

</div>