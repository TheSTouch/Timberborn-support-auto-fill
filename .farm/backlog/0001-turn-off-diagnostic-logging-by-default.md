- [!] #1 Turn off diagnostic logging by default
      - `DiagnosticLogging` in `PlatformAutofillService` is hardcoded to `true`, flooding the player log in every session
      - accept: `DiagnosticLogging` defaults to `false`; gate passes
      from: preparation, stage backlog, signed 2026-11-02 by owner; read .farm/preparation/
      farm: branch farm/1-turn-off-diagnostic-logging-by-default is pushed, but origin is not on a forge the farm can open a pull request on (see farm-forge of) — session 'farm-Timberborn-support-auto-fill-1' still live, answer it from Remote Control
