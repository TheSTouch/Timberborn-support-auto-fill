- [!] #3 Expose max-support-size selector in the UI
      - `SetMaxSupport(int index)` exists on the service but nothing in the fragment exposes it; players cannot limit autofill to single or double platforms
      - accept: the tool fragment shows a control that sets the max support index (0/1/2); the selected value is used by the next placement; gate passes
      from: preparation, stage backlog, signed 2026-11-02 by owner; read .farm/preparation/
      farm: The repository's .claude settings could redirect or re-key the session (.claude/settings.json sets hooks). Remove those keys, or set repo_claude_settings: ignore in .farm/project.yml so the lane sets the file aside for sessions. No session was started.
