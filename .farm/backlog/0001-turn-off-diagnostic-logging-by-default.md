- [ ] #1 Turn off diagnostic logging by default
      - `DiagnosticLogging` in `PlatformAutofillService` is hardcoded to `true`, flooding the player log in every session
      - accept: `DiagnosticLogging` defaults to `false`; gate passes
      from: preparation, stage backlog, signed 2026-11-02 by owner; read .farm/preparation/
      farm: stalled — silent for 2700s with no question on screen, so the session was closed and the item requeued. AT RISK when it stopped: 0 uncommitted file(s), 1 commit(s) not on main — kept on farm/stalled-1, redo from there rather than from scratch
