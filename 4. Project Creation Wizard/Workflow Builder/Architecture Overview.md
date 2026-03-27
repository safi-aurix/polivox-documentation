The workflow builder is composed of four main components that work together:

|**Component**|**File**|**Purpose**|
|---|---|---|
|StepWorkflowBuilder|StepWorkflowBuilder.tsx|Main orchestrator — manages state, coordinates sub-components|
|WorkflowNodePalette|WorkflowNodePalette.tsx|Left sidebar — draggable node type cards|
|WorkflowCanvas|WorkflowCanvas.tsx|Center — React Flow canvas for visual editing|
|WorkflowPropertyPanel|WorkflowPropertyPanel.tsx|Right sidebar — node configuration panel|
|WorkflowNode|nodes/WorkflowNode.tsx|Custom node rendering (standard + condition diamond)|

The layout is a three-panel design: the palette on the left (224px), the interactive canvas in the center (flexible width), and the property panel on the right (320px, shown only when a node is selected).