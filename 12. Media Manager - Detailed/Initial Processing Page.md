This page is the Media Manager's primary workspace for preparing raw audio recordings.

#### Page Header & Responsibilities
- Merge individual speaker tracks into a single mixed audio file
- Normalize audio levels across all speakers for consistent volume
- Trim silence at the beginning and end of recordings
- Apply any required audio cleanup (noise reduction, equalization)
- Submit processed audio to QC1 for quality review

#### Statistics & Filters
Three stat cards show Total Sessions, Pending Processing, and Re-processing Required (sessions flagged by QC). Clickable status filters, language and category dropdowns, and a search bar let the MM narrow down the session list.

#### Session Table
A paginated table lists sessions with columns for Topic, Session ID, Category, Speakers, Duration, Languages, Tracks, and Status. Sessions flagged by QC show a 'Changes from QC' badge. Each row has an 'Open & Process' button.

![[initial_processing_sessions.png]]

#### Initial Processing Detail View
A full-screen modal provides the complete audio processing workspace.

**_Toolbar_**
Two buttons at the top allow uploading replacement tracks or downloading all tracks as a ZIP archive. The download tooltip shows the ZIP file structure (speaker WAVs, mixed track, and metadata JSON).

**_QC Feedback Alert_**
If this session is returning from QC with issues, an amber alert box displays the QC reviewer's comments so the MM knows exactly what to fix.

**_Speaker Tracks Section_**
Individual cards for each speaker track (SPK1, SPK2, etc.) are displayed in a two-column grid. Each card contains:
- A download and replace button for the individual track
- A vertical gain slider allowing level adjustment from -20 dB to +20 dB with real-time dB readout
- An interactive waveform player where the MM can click and drag to select silence regions for removal
- A list of silenced segments shown as time-range badges (e.g., '0:03 — 0:08') with individual delete buttons and a 'Clear all' option

**_Normalize Final Mix_**
A dedicated card with a horizontal slider sets the target peak level for the final mix (range: -10 dB to 0 dB). A waveform preview shows the final normalized result.

**_Final Merged Audio_**
A preview card shows the merged waveform of all speaker tracks combined, with download and replace options.

**_Submit Action_**
A 'Generate & Send for Quality Check' button at the bottom submits the processed session to QC1. A success toast confirms the submission and the modal closes.

![[initial_processing_detailed_view.png]]