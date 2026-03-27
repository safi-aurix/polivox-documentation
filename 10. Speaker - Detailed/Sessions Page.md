The sessions page is the speaker's main workspace, organized into two tabs: Live Sessions and Scheduled Sessions.

#### Live Sessions Tab
Displays a responsive grid of topic cards for sessions currently accepting participants. Each card shows:
- Category badge (color-coded: indigo for Natural Conversation, amber for Scenario-Based, emerald for Interview Style)
- Topic title
- Language pair shown as adjacent badges with an arrow between them
- Participant progress bar showing filled slots (e.g., '3 of 6 speakers'), with a 'FILLING FAST' badge when nearly full
- 'Join Session' button that navigates to the waiting lobby

![[live_sessions_page.png]]
#### Waiting Lobby
After clicking 'Join Session', the speaker enters a waiting lobby. The lobby displays:
- The topic's title, category, and language pair at the top
- A 6-slot speaker grid showing filled slots (avatar, name, language badge) and empty slots (dashed circle, 'Waiting...')
- The current speaker's slot is labeled 'You'
- A status indicator that changes dynamically:
	- While waiting: 'Waiting for speakers to join...' with a clock icon
	- When all 6 slots fill: a 5-second countdown begins automatically with a red pulsing indicator and 'Prepare your microphone...' prompt
	- When countdown reaches 0: 'Starting recording...' with green indicator, then auto-transitions to recording room
- A 'Leave Queue' button to exit before recording starts

![[waiting_lobby.png]]
#### Recording Room
The recording room provides a timed 5-minute recording session interface:
- A pulsing red 'Recording' indicator with microphone icon
- A large countdown timer (5:00 → 0:00) that changes color: green when > 2 min, yellow at 1–2 min, red when < 30 seconds
- A conversation script card showing the dialogue lines for the session, with lines advancing automatically based on elapsed time — the current line is highlighted, past lines are dimmed, and future lines are at reduced opacity
- A speakers section showing all participants as colored avatars with names and language badges
- An 'End Recording' button (red) to finish early — otherwise recording auto-completes at 5 minutes
- On completion: a success toast appears ('Recording completed successfully!') and the speaker returns to the browse view

![[recording_room.png]]
#### Scheduled Sessions Tab
Shows two sections: Upcoming and Past Sessions. Each session card displays:
- Status badge (Upcoming/blue, Active/green pulsing, Recorded/green check, Rejected/red)
- A 'Re-record' badge on rejected sessions
- Topic title and language pair badges
- Scheduled date and time with calendar icon
- Participant avatars (up to 4) and speaker count (e.g., '4/6 speakers')
- A 'Join' button that appears only for upcoming sessions within 15 minutes of start time

![[scheduled_session_tab.png]]