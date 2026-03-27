The QC1 page is the full task list for initial audio quality review. It is accessed from the sidebar or the dashboard 'View all' link.

#### Page Header & Responsibilities
The page displays a role information box outlining QC1 duties:
- Listen to the full mixed audio recording for each session
- Verify audio is at least 5 minutes long with clear speech from both speakers
- Check for technical issues: echo, clipping, background noise, or silence gaps
- Confirm both languages are used appropriately per the topic prompt
- Flag issues with detailed comments or approve to send to noise processing

#### Statistics & Filters
Three stat cards show Total in QC1, Pending Review, and Issues Found. Below, clickable status badge filters (All / Pending Review / Issues Found) let the reviewer narrow the list. Additional dropdowns filter by language pair and topic category, and a search bar supports lookup by topic title, session ID, or category.

#### Session Table
A paginated table lists all QC1 sessions with columns for Topic, Session ID, Category, Speakers, Duration (MM:SS), Languages, Tracks, and Status. Each row has a 'Review' button that opens the detail view.

![[qc1_session_table.png]]

#### QC1 Detail View (Review Modal)
The detail view is a large scrollable modal where the reviewer evaluates a single session. It contains the following sections:

**_Session Header_**
A sticky header shows the session's topic title, a 'QC 1 — Audio Quality' badge, the recording date and time, session ID, category, language pair, duration, and speaker count.

**_Previous QC1 Issues Alert_**
If the session was previously flagged and is returning for re-review, an amber warning box displays the original QC1 comments so the reviewer can check whether the reported problems have been fixed.

**_Mixed Audio Player with Waveform_**
The primary review tool is a mixed audio player with an interactive waveform. The reviewer listens to the combined recording and can drag on the waveform to create 'flagged regions' — timestamped segments that mark where issues occur. Each flagged region appears as a visual marker on the waveform and is listed below the player with its time range (e.g., '0:42 — 1:15') and an editable comment field where the reviewer describes the specific issue. Regions can be individually removed.

![[selected_flagging_qa.png]]

**_Audio Quality Checklist_**
The checklist assigned by Project Manager on [[4. Project Creation Wizard/Workflow Builder/Workflow Builder|Workflow Builder]] in the [[Property Panel (Node Configuration)]] of Quality Checker.

Items turn green with a checkmark icon when completed. A counter shows progress (e.g., '3/5 checked'). All required items must be checked before the 'Good to Go' approval button becomes enabled.

![[initial_qc_checklist.png]]

**_Individual Speaker Tracks_**
A collapsible section shows individual audio players for each speaker's track (e.g., SPK1, SPK2). This helps the reviewer isolate speaker-specific issues like low volume or background noise on a single channel.

**_Decision Actions_**
The modal footer offers two actions:
- **Good to Go** — Approves the session and sends it to the noise processing stage. Disabled until all checklist items are checked.
- **Flag Issues** — Opens an issue form with a text area for describing the problems. Any waveform flagged regions are automatically included with their timestamps and comments. Sends the session back to the Media Manager for reprocessing.

![[qc1_detailed_view.png]]