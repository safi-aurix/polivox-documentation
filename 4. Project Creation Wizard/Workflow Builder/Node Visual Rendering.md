#### **1. Standard Nodes**

Standard nodes (all types except Condition) render as rounded rectangles with a colored left border matching the node type. The content includes:
- Icon in a colored square (top-left) with the node label beside it
- Optional description text below the label (gray, truncated)
- Subtype badge for QC and MM nodes (e.g., 'Initial Processing QA')
- Recording Room: 'Accepts: 2, 6, 10 speakers' badge showing valid counts
- Checklist indicator for QC nodes (e.g., '3 checklist items')
- Assigned staff indicator showing first 2 names + '+N more'
- Tasks preview showing first 3 items + '+N more'

Handles: one input handle on the left (target) and one output handle on the right (source), both colored to match the node type.

![[standard_node.png]]

#### **2. Condition Nodes**

Condition nodes have a distinctive diamond shape (rotated square) to visually distinguish them from standard nodes. They display:
- GitBranch icon in a colored circle (center)
- Node label (bold, centered)
- Branching field name (e.g., 'speakerCount')
- Path count indicator (e.g., '3 paths')

The diamond dynamically grows taller based on the number of paths (minimum height: 140px, formula: max(140, pathCount × 36 + 80)). Each path creates a separate colored output handle on the right side, distributed vertically with equal spacing. Path labels are displayed next to their handles.

See [[Condition Branching System]] for more info.

![[condition_node.png]]