The canvas is the central interactive area where nodes are placed and connected. It supports:
- **Drag-and-Drop Placement** — Nodes from the palette are dropped onto the canvas at the desired position
- **Node Selection** — Clicking a node selects it and opens the property panel on the right. Clicking the canvas background deselects.
- **Edge Drawing** — Dragging from an output handle (right side of node) to an input handle (left side of another node) creates a connection edge.
- **Pan and Zoom** — The canvas supports mouse wheel zoom and click-drag panning.
- **Minimap** — A small overview map in the bottom-right corner for navigation in large workflows.
- **Background Grid** — A dot grid with 16px spacing provides visual alignment reference.

Default edge styling uses gray stroke (#94a3b8), 2px width, with animation. Edges from condition nodes use path-specific colors and labels.

![[workflow_builder_canvas.png]]