# gen2-parts

The MODULITH part assets served to the planner over GitHub Pages:

- `parts/<length>/*.lib.glb` — the part library the 3D stage loads (meshopt-compressed GLBs, one folder per collection length).
- `img/parts/*.png` — the part thumbnails the parts list and the part card show.

They were moved here from the viewer repository (`viewer/parts` and `viewer/img/parts`) on 2026-10-12 so the merged planner repo stays small and the assets deploy on their own. The planner points at this host through one `PARTS_BASE` setting. Pages serves every file with `Access-Control-Allow-Origin: *`, which cross-origin GLB loading needs.
