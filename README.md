# Aster VRM Material Editor

A lightweight, Android-friendly browser editor for **VRM 0.x only**.

## Features
- Load and preview VRM 0.x locally in the browser.
- Inspect material slots and edit base color, alpha, texture, alpha mode and double-sided state.
- Convert the selected material to Unlit.
- **Convert ALL materials used by all mesh primitives to Unlit** in one action, including multiple material slots.
- Preserve base-color texture references, base-color factors, alpha mode/cutoff and double-sided settings.
- Export the edited model as a VRM/GLB file.
- Reject VRM 1.0 files explicitly.

## Unlit conversion
The bulk conversion updates the glTF `KHR_materials_unlit` extension and aligns the VRM 0.x `extensions.VRM.materialProperties` entries. It chooses the VRM 0.x Unlit shader variant from the material alpha mode and texture usage. It does not add fake UniVRM metadata.

## Privacy
Model processing runs in the browser. The model is not uploaded by this page.

## Important
This is a preview build. Test exported files in the VRM applications you use. Compatibility with every VRM 0.x importer is not guaranteed.
