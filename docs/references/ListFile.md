# ListFile

The `listfile.txt` is a plaintext mapping between numeric file IDs and real file paths inside the WoW game client. It is used by modern retail builds to locate game assets, including:

- Icons (`.blp`)
- Models (`.m2`)
- Skins (`.skin`)
- Textures (`.blp`, `.dds`)
- Animation files (`.anim`, `.skel`)

This system replaces the legacy MPQ path system used in 3.3.5a and earlier.

---

## Format

Each line in `listfile.txt` looks like:

```text
<FileDataID>;<RelativePath>
```
---






























<div style={{ fontSize: '0.9em', color: 'var(--ifm-color-content-secondary)' }}>

### 🖋️ Credits

This documentation was written and maintained by [**Sylian**](https://github.com/Sylian1337), creator of **SylCore** and educator on [YouTube](https://www.youtube.com/@DEVSylian).

If you use this, consider contributing back, or showing your support to the authors 🙏

</div>