# FileDataID

The `FileDataID` field references any asset file stored in the WoW client’s CASC system. This includes `.m2`, `.skin`, `.blp`, `.skel`, and other file types used in models, textures, and UI.

It is resolved using the `listfile.txt` mapping system.

---

### How it Works

The value is matched against entries in the `listfile.txt`, which maps numeric file IDs to client file paths. This is similar to how MPQ file indexing worked in 3.3.5, but in retail clients, the file structure is abstracted and all lookups are done by ID.

---

### Where It’s Used

Commonly used in:

- `ModelFileData.db2`

Each `FileDataID` maps to a client-side file such as:

```text
7233207;models/unknown/unk_exp10_7233207/7233207.m2
4323455;interface/icons/inv_ring_progenitorraid_01_red.blp
```

To understand how this mapping works, refer to the [Listfile Reference ->](/docs/references/ListFile.md)

---

### Usage Aliases
Different DB2 tables and fields use context-specific names for FileDataID, depending on the type of asset being referenced.

| Field Name          | Used For          | File Types              |
| ------------------- | ----------------- | ----------------------- |
| `IconFileDataID`    | Item/spell icons  | `.blp`                  |
| `ModelFileDataID`   | 3D models         | `.m2`, `.skin`, `.skel` |
| `TextureFileDataID` | Terrain/textures  | `.blp`, `.dds`          |
| `FileDataID`        | Generic reference | Varies                  |

---

### Important Notes
The ID is numeric — the file path is never stored in the DB2.

You must cross-reference the ID using the client’s listfile or tools like WoW.tools.

Some IDs point to virtual paths (auto-generated during client patching).

---

### Related
 - [Listfile Reference ->](/docs/references/ListFile.md)

---

<div style={{ fontSize: '0.9em', color: 'var(--ifm-color-content-secondary)' }}>

### 🖋️ Credits

This documentation was written and maintained by [**Sylian**](https://github.com/Sylian1337), creator of **SylCore** and educator on [YouTube](https://www.youtube.com/@DEVSylian).

If you use this, consider contributing back, or showing your support to the authors 🙏

</div>