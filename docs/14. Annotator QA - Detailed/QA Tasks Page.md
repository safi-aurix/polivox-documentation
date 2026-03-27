#### Page Header & Responsibilities
- Spot-check annotation accuracy against the original audio
- Verify speaker IDs and language tags are correctly assigned
- Check timestamp precision and segment boundaries
- Run overlap detection and validate flagged segments
- Approve accurate annotations or send back with specific feedback

#### Statistics & Filters
Three stat cards (Total in QA, Pending QA, Resubmitted) summarize the queue. Clickable status filters, language and category dropdowns, and search bar provide filtering.

![[annotator_qa_sessions.png]]
#### QA Detail View (Review Modal)
The QA review modal provides tools for thorough annotation verification.

**_Session Header_**
A sticky header shows the topic title, 'Annotation QA' badge, optional 'Resubmitted' badge, recording date, session ID, and session metadata. Also displays the count of annotation turns for quick reference.

**_Mixed Audio & Speaker Tracks_**
Same audio playback tools as the annotator view — a mixed audio player and collapsible individual speaker tracks — so the reviewer can listen while verifying annotations.

**_Annotation Turns Table (Read-Only)_**
All annotation turns are displayed in a read-only table with columns for turn number, speaker, start time, end time, language, and transcription. Unlike the annotator's editable view, the QA reviewer cannot modify turns — they can only select them for feedback. Clicking a row selects it (highlighted with an amber left border and amber background). Multiple turns can be selected simultaneously, building a list of problematic turns to reference in feedback.

![[annotation_turns.png]]

**_Feedback Thread_**
The feedback system allows the QA reviewer to communicate with the annotator at a granular turn level:
- The reviewer selects problematic turns by clicking rows in the annotation table
- Selected turns appear as removable amber badges in the feedback composer (e.g., 'Turn 3', 'Turn 7')
- The reviewer writes a description of the issues in a text area
- Clicking 'Send' creates a feedback message with the turn references attached, and returns the session to the annotator
- All previous messages are displayed in the thread — QA messages (purple) and annotator replies (blue)
- Clicking a turn badge in any message jumps to and highlights that turn in the table for 2 seconds

![[feedback_thread.png]]

**_Overlap Detection_**
A built-in analysis tool detects overlapping speech segments. The reviewer clicks 'Run Overlap Check' to trigger a scan. After a brief analysis, results are displayed showing:
- Time range of each detected overlap (e.g., '1:23 — 1:28')
- The speakers involved (e.g., 'SPK1 + SPK2')
- An overlap type badge: 'Real Overlap' (amber) or 'False Positive' (gray)
- A toggle button to reclassify each overlap between real and false positive

A summary at the bottom shows the total real overlaps and false positives.

![[overlap_detection.png]]

**_Annotation Quality Checklist_**
A four-item checklist ensures systematic evaluation:
- Accurate turn boundaries (start/end times)
- Correct speaker labels (SPK1–SPK6)
- Correct language tags per turn
- Acceptable transcription quality

![[annotation_quality_checklist.png]]

All items must be checked to enable the approval button. A counter shows progress and an 'All passed' badge appears when complete.

**_Decision Actions_**
- **Approve — No Fixes Required** — Moves the session to ready-for-delivery status. Disabled until all checklist items are checked.
- **Send Feedback (via thread)** — Returns the session to the annotator with linked turn references. The annotator sees which specific turns need attention.

![[annotator_qa_detailed_view.png]]