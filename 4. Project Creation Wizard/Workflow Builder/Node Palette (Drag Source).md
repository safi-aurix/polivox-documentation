The left sidebar displays all eight node types as draggable cards. Each card shows the node's icon (color-coded), label, and a short description. A grip handle icon indicates that the card is draggable.

To add a node to the workflow, the user drags a card from the palette and drops it onto the canvas. The system:
- Captures the palette item data via HTML5 drag-and-drop (MIME type: application/workflow-node)
- Converts the mouse drop position from screen coordinates to React Flow canvas coordinates
- Creates a new WorkflowNode with a unique ID (format: node-{counter}-{timestamp})
- Initializes the node with default data (empty tasks, default condition config for condition nodes)