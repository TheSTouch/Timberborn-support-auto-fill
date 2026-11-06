- [ ] #1 Turn off diagnostic logging by default
      - `DiagnosticLogging` in `PlatformAutofillService` is hardcoded to `true`, flooding the player log in every session
      - accept: `DiagnosticLogging` defaults to `false`; gate passes
      from: preparation, stage backlog, signed 2026-11-02 by owner; read .farm/preparation/
