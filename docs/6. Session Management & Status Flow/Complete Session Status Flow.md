**This flow might change for different projects.**

Sessions progress through up to 24 distinct statuses representing the full production pipeline. The primary flow is:

| **Status**             | **Phase**                     | **Responsible Role** |
| ---------------------- | ----------------------------- | -------------------- |
| recorded               | Recording                     | Speaker              |
| initial-processing     | Audio Processing              | Media Manager        |
| reprocessing-required  | Audio Processing (rework)     | Media Manager        |
| qc1-pending            | Quality Control 1             | Quality Checker      |
| qc1-approved           | QC1 Passed                    | —                    |
| qc1-issues             | QC1 Issues (PM Review)        | Project Manager      |
| noise-processing       | Noise Injection               | Media Manager        |
| noise-reprocessing     | Noise Rework                  | Media Manager        |
| qc2-pending            | Quality Control 2             | Quality Checker      |
| qc2-approved           | QC2 Passed                    | —                    |
| qc2-issues             | QC2 Issues (PM Review)        | Project Manager      |
| annotation-pending     | Annotation                    | Annotator            |
| annotation-issues      | Annotation Issues (PM Review) | Project Manager      |
| annotation-resubmitted | Annotator Resubmitted         | Annotator QA         |
| annotation-qc-pending  | Annotation QA Review          | Annotator QA         |
| annotation-qc-approved | Annotation QA Passed          | —                    |
| ready-for-delivery     | Ready for Export              | Project Manager      |
| exported               | Exported to Drive             | —                    |
| rejected               | Rejected                      | —                    |
| re-record-required     | Re-recording Needed           | Speaker              |

### **Workflow Differences by Project Type**

- **2-Speaker Projects** — Include the noise injection step. Sessions go through QC2 after noise processing.
- **6-Speaker Projects** — Skip the noise injection step entirely. Sessions move directly from QC1 to annotation.