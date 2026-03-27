#### Page Header & Responsibilities
- Listen to each audio segment and transcribe speaker turns accurately
- Tag each turn with the correct speaker ID and language code
- Mark precise start and end timestamps for every segment
- Identify and label overlapping speech between speakers
- Follow the annotation guidelines for formatting and language tagging

#### Statistics & Filters
Four stat cards (Total Assigned, Pending, Issues, Resubmitted) provide a workload summary. Clickable status filters, language and category dropdowns, and a search bar narrow the session list.

#### Session Table
A paginated table with columns for Topic, Session ID, Category, Speakers, Duration, Languages, Tracks, and Status. Sessions with issues show a red badge; resubmitted sessions show a blue badge. Each row has an 'Annotate' button.

![[annotator_sessions.png]]

#### Annotation Detail View (Editor Modal)
The annotation editor is a large scrollable modal that serves as the annotator's primary workspace. It contains several integrated sections:

**_Session Header_**
A sticky header shows the topic title, status badges ('Annotation' + 'Needs Revision' or 'Resubmitted' if applicable), recording date, session ID, category, languages, duration, and participant count.

**_Feedback Thread_**
If the session is returning from QA review, a feedback thread displays all messages exchanged between the annotator and QA reviewer. QA messages appear with a purple background and 'QA Reviewer' badge; annotator messages appear with a blue background and 'Annotator' badge. Each message may include linked turns displayed as amber badges — clicking a turn badge scrolls to and highlights that turn in the editor below. The annotator can reply to QA feedback by typing a message and clicking Send.

![[feedback_thread_annotator.png]]

**_Mixed Audio Player_**
A full audio player with waveform visualization shows the combined recording. The annotator listens while creating turns, using play/pause controls, a progress bar, and elapsed/remaining time display.

**_Individual Speaker Tracks_**
A collapsible section shows separate audio players for each speaker's track. This helps the annotator identify individual speakers when transcribing and resolve ambiguous segments.

**_Transcript Reference_**
A collapsible section displays an auto-generated reference transcript (if available). Each segment shows a timestamp, a color-coded speaker name, and the segment text in a speech bubble. A speaker legend with colored dots is shown at the bottom. This reference is read-only and serves as a starting point for annotation.

![[transcript_reference_annotator.png]]

**_Annotation Turns Editor_**
The main editing area where the annotator creates and manages individual transcription turns. The toolbar offers two options:
- **AI Transcribe** — Auto-generates annotation turns from the reference transcript, pre-filling speaker IDs, timing, languages, and text. A toast confirms the action.
- **Add Turn** — Manually adds a new blank turn below the last one, with the start time set to the previous turn's end time.

![[annotation_turns_annotator.png]]

Each turn is a collapsible card with the following editable fields:
- Turn label (e.g., Turn 1, Turn 2) — automatically numbered
- Speaker dropdown (SPK1, SPK2, ... based on participant count)
- Language dropdown (language codes extracted from the session)
- Start time and End time inputs in MM:SS format
- Transcription text area for the spoken content
- Delete button to remove the turn (remaining turns are renumbered)

Turns that were flagged by QA are visually highlighted with an amber border and a 'QA flagged' badge, making it immediately clear which turns need attention.

**_Submission_**
A 'Submit for QC' button (disabled if no turns exist) sends the annotation to the Annotator QA reviewer. A success toast confirms the submission.

![[annotation_detailed_view.png]]