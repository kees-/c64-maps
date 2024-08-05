Unsorted depot for the increasing number of tester maps on [my fork of Celeste64](https://github.com/kees-/Celeste64).

## Tooling

### Blender template

Contains a blender application template for creating heightmaps in direct conjunction with [kees-/io_export_qmap](https://github.com/kees-/io_export_qmap). Place the `Celeste64` directory present in `tooling` into `scripts/startup/bl_app_templates_user` of blender conf. Then, "Celeste64" will be a template option when creating new blender files.

"One-click" mapping: open an image into the texture that's visible in the sidebar when the template is used. The heightmap will be immediately visible with sensible defaults. Change the values in the modifier pane from there, such as displacement strength, decimation ratio, or subdivision levels.

![](https://github.com/user-attachments/assets/91b8c3a3-3805-4c86-acdf-fdef77526803)

Use io_export_qmap (*with all the right settings) and the map will be almost ready to play. The only other necessity is creating a `PlayerSpawn` entity with `name` set to `Start` somewhere on the mesh surface, which can be done in blender with an empty object or trenchbroom.
