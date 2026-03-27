The workflow builder's state is managed through React Flow hooks (useNodesState, useEdgesState) inside StepWorkflowBuilder. The data flow works as follows:
- Node Creation: Palette drag → Canvas drop → new node added to state
- Node Update: Property panel change → handleNodeUpdate → updates both nodes array and selectedNode
- Node Delete: Delete button → removes node and all connected edges → deselects
- Edge Creation: Handle drag → onConnect → evaluates condition paths → applies styling → adds edge
- Sync to Parent: When property panel closes → syncToParent → onChange callback sends current nodes/edges to CreateProject parent component