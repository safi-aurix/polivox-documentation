Each node represents a state in the [[Session Management & Status Flow]].

The system defines eight distinct node types, each representing a different role or function in the processing pipeline:

|**Node Type**|**Icon**|**Color**|**Description**|
|---|---|---|---|
|Speaker|Mic|Indigo (#6366f1)|Language speaker participant in recording sessions|
|Recording Room|Radio|Sky Blue (#0ea5e9)|Room configuration where speakers record|
|Media Manager|FileAudio|Amber (#f59e0b)|Audio file processing (initial or noise)|
|Quality Checker|ShieldCheck|Emerald (#10b981)|Audio and data quality review|
|Annotator|PenTool|Violet (#8b5cf6)|Transcription and linguistic annotation|
|Annotator QA|ClipboardCheck|Pink (#ec4899)|Annotation accuracy review|
|Processing Step|Cpu|Slate (#64748b)|Automated processing (noise reduction, etc.)|
|Condition|GitBranch|Orange (#f97316)|Branch workflow based on dynamic conditions|