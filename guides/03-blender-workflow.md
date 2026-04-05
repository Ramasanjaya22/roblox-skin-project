# Blender Workflow - Roblox Skin Creation

## Prerequisites

### Software
- Blender 3.x or 4.x LTS (free)
- Roblox Studio (free)

### Skills Needed
- Basic 3D modeling
- UV mapping basics
- Texture creation (optional)

---

## Project Setup

### Blender Settings for Roblox

1. **Unit Preferences**
   - Scene → Units → Metric
   - Unit Scale: 1.0

2. **Viewport**
   - Switch to "Material Preview" mode
   - Enable "Studio Lighting" for preview

3. **Export Preset**
   - Save as FBX default
   - Include: Mesh, Armature
   - Apply scale: All Local

---

## Creating Your First Skin

### Step 1: Base Mesh (Hair Example)

```
1. Add → Mesh → Plane
2. Enter Edit Mode (Tab)
3. Model the basic hair shape
   - Use Extrude (E)
   - Use Loop Cuts (Ctrl+R)
4. Add thickness with Solidify modifier
5. Smooth with Subdivision Surface
```

### Step 2: Rigging (Optional)

For R15/R6 compatibility:
```
1. Import Roblox rig (download from DevForum)
2. Parent mesh to bones
3. Weight paint
4. Test deformation
```

### Step 3: UV Unwrapping

```
1. Enter Edit Mode
2. Select all (A)
3. Press U → Smart UV Project
4. Adjust islands in UV Editor
5. Minimize overlap
```

### Step 4: Texturing

```
Option A: Vertex Colors (Simpler)
- Paint directly on mesh
- No texture file needed

Option B: Image Texture
- Create UV map layout
- Paint in Photoshop/Procreate
- Export as PNG (1024x1024 recommended)
```

### Step 5: Export

```
File → Export → FBX (.fbx)

Settings:
- Format: FBX
- Apply Scalings: All Local
- Apply Transform: CHECKED
- Mesh: CHECKED
- Armature: (if used)
- Limit to: Selected Objects
```

---

## Common Techniques

### Low Poly Guidelines
- Target: 2,000-5,000 polygons
- Use flat shading for stylized looks
- Bake details from high-poly if needed

### Optimization
- Remove internal geometry
- Merge vertices where possible
- Use materials efficiently (max 3-4)

### Animation Ready
- Keep mesh deformation simple
- Test in Roblox Studio before finishing
- Avoid complex shape keys

---

## Troubleshooting

| Issue | Solution |
|-------|----------|
| Mesh broken on import | Check normals (shift+N) |
| Wrong scale in Roblox | Apply all transforms (Ctrl+A) |
| Texture not showing | Use proper material setup |
| Performance lag | Reduce polygon count |
| Color looks wrong | Check color space (sRGB) |

---

## Roblox-Specific Tips

1. **Test Early** - Import to Roblox frequently
2. **Keep It Simple** - Don't overcomplicate
3. **Follow Guidelines** - Check Roblox content policy
4. **Naming Convention** - Clear names for parts

---

## Export Checklist

- [ ] Apply all transforms
- [ ] Check normals are correct
- [ ] UVs don't overlap
- [ ] Polygon count under 10k
- [ ] File size under 5MB
- [ ] Export as FBX

---

## Next Steps

- Continue: `resources/tools.md`
- See: `templates/design-brief.md`

---

*Last Updated: 2026*