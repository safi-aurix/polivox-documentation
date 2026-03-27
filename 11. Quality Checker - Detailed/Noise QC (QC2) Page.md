The QC2 page follows the same structure as QC1 but focuses on validating the noise layer applied to the audio.

#### Page Header & Responsibilities
- Review the noise-injected audio to ensure environmental sounds are realistic
- Verify noise levels don't overpower speaker voices
- Check that noise transitions are smooth and natural
- Confirm the original speech quality is preserved after noise addition
- Flag issues for the Media Manager to fix or approve for annotation

![[noise_qc_sessions.png]]
#### QC2 Detail View (Review Modal)
The QC2 detail view is structurally similar to QC1 with these key differences:

**_Noise Layer Information_**
An information card displays the type of noise applied (e.g., 'Office Ambience') and the intensity level (e.g., '20%'), giving the reviewer context for what to expect.

**_Audio With Noise Player_**
The primary waveform player shows the noise-injected audio. The reviewer can drag to flag problem regions just as in QC1.

**_Clean Mixed Audio Reference_**
A collapsible section provides the original clean audio (before noise was added) so the reviewer can A/B compare and assess whether the noise layer has degraded the original quality.

**_Noise Quality Checklist_**
The checklist assigned by Project Manager on [[4. Project Creation Wizard/Workflow Builder/Workflow Builder|Workflow Builder]] in the [[Property Panel (Node Configuration)]] of Quality Checker.

Items turn green with a checkmark icon when completed. A counter shows progress (e.g., '3/5 checked'). All required items must be checked before the 'Good to Go' approval button becomes enabled.

![[noise_quality_checklist.png]]

**_Decision Actions_**
- **Approve & Send to Annotation** — Moves the session to the annotation queue. Requires all checklist items checked.
- **Flag Issue** — Opens an issue form and sends the session back to the Media Manager for noise rework, including any flagged waveform regions.

![[noise_qc_detailed_view.png]]
