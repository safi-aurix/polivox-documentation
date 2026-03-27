When a node is selected, the right sidebar (320px) opens to show all configurable properties for that node type. The panel adapts its content based on the node's role.

#### Universal Properties (All Nodes)
- Label — text input to customize the node's display name
- Description — optional text input (hidden for condition nodes)

#### Recording Room Properties
- **Acceptable Speaker Counts** — A numeric input with add/remove functionality. Values appear as removable badges. Defines which speaker configurations are valid for this recording room (e.g., exactly 2, 6, or 10 speakers).

#### Quality Checker Properties
- **QC Subtype** — Dropdown to select '[[Initial Processing QA]]' or '[[Noise Processing QA]]'.
- **QC Checklist** — Add custom verification items. Each item has a label and a required/optional toggle. QC reviewers use this checklist when evaluating sessions. See [[Initial QC (QC1) Page]] where this checklists will be visible.

#### Media Manager Properties
- **Processing Type** — Dropdown to select '[[Initial Processing]]' or '[[Noise Processing]]'.

#### Condition Node Properties
- **Branch On** — Dropdown to select the branching field (Speaker Count, Language Pair, Recording Type, Custom).
- **Path Management** — Add new paths (label + value), edit existing path labels, remove paths. Each path automatically receives a color from the 8-color palette.

#### Tasks/Responsibilities (Non-Condition Nodes)
- A free-form list of tasks. Add task descriptions via a text input. Each task appears as a removable item. The first 3 tasks are previewed on the node card.

#### Delete Node
- A red destructive button at the bottom of every property panel allows deleting the selected node and all its connected edges.