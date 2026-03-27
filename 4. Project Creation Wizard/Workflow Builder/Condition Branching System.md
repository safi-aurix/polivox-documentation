The condition node is the most complex node type, enabling multi-path workflow branching. It allows the workflow to diverge into different processing paths based on a runtime field value.

#### **1. Configuration**
A condition node is configured with:
- **Branch Field** — The data field to evaluate. Options: Speaker Count, Language Pair, Recording Type, or Custom Field.
- **Paths** — Each path defines a possible output branch with:
	- Label — display name (e.g., '2 Speakers')
	- Value — the matching value (e.g., '2')
	- Color — automatically assigned from 8-color palette: Emerald, Blue, Amber, Red, Violet, Pink, Cyan, Lime

#### **2. How Branching Works**
When a condition node has paths configured:
- Each path creates a separate output handle on the right side of the diamond
- Handles are color-coded and labeled to distinguish branches
- When a user draws an edge from a specific path handle to a target node, the edge inherits that path's color and label
- This creates a visually clear multi-path workflow where each branch is identifiable by color

Example: A condition node branching on 'Speaker Count' might have three paths — '2 Speakers' (green), '6 Speakers' (blue), '10 Speakers' (amber) — each leading to different downstream processing nodes.