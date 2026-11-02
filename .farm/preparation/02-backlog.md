# Its backlog

Role: intake. Version 1, signed 2026-11-02T19:33:27Z by owner.

# Backlog

- [ ] Turn off diagnostic logging by default
  - `DiagnosticLogging` in `PlatformAutofillService` is hardcoded to `true`, flooding the player log in every session
  - accept: `DiagnosticLogging` defaults to `false`; gate passes

- [ ] Add a keyboard shortcut to toggle autofill
  - Currently the only way to toggle is clicking the UI button; a hotkey (e.g. a configurable key) would let players toggle without moving the cursor away from placement
  - accept: pressing the bound key toggles autofill on/off while a supported tool is active; gate passes

- [ ] Expose max-support-size selector in the UI
  - `SetMaxSupport(int index)` exists on the service but nothing in the fragment exposes it; players cannot limit autofill to single or double platforms
  - accept: the tool fragment shows a control that sets the max support index (0/1/2); the selected value is used by the next placement; gate passes

- [ ] Persist the autofill toggle state across sessions
  - `IsEnabled` resets to `false` on every game load, so players must re-enable each session
  - accept: the toggle state survives exiting and re-entering a game session; gate passes

- [ ] Support single-click placements
  - README lists "only triggers during drag-placement" as a known limitation; single-click placements on elevated terrain are ignored
  - accept: placing a supported block with a single click on terrain with a vertical gap queues supports the same way drag placement does; gate passes
