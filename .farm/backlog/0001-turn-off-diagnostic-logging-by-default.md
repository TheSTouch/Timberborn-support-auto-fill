- [!] #1 Turn off diagnostic logging by default
      - `DiagnosticLogging` in `PlatformAutofillService` is hardcoded to `true`, flooding the player log in every session
      - accept: `DiagnosticLogging` defaults to `false`; gate passes
      from: preparation, stage backlog, signed 2026-11-02 by owner; read .farm/preparation/
      farm: The repository's .claude settings could redirect or re-key the session (.claude/settings.json sets hooks). Remove those keys, or set repo_claude_settings: ignore in .farm/project.yml so the lane sets the file aside for sessions. No session was started.
