A speaker must pass through three distinct logical gates to be considered for a "Match":

1. **Linguistic Gate:** * The speaker’s `Language Profile` must contain the **Source** and **Target** languages defined in the [[Project Creation Wizard]].
    - _Logic:_ `(User.Languages.includes(Project.Source)) AND (User.Languages.includes(Project.Target))`
2. **Availability Gate:**
    - The speaker must be "Active" and not currently engaged in a maximum number of concurrent sessions.
3. **Performance Gate:**
    - Speakers with a **Flagged** status are automatically excluded.
    - Speakers with a **Star Rating < 3.0** are deprioritized or excluded based on PM settings.