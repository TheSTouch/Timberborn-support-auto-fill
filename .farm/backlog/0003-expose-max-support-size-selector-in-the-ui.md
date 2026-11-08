- [x] #3 Expose max-support-size selector in the UI
      - `SetMaxSupport(int index)` exists on the service but nothing in the fragment exposes it; players cannot limit autofill to single or double platforms
      - accept: the tool fragment shows a control that sets the max support index (0/1/2); the selected value is used by the next placement; gate passes
      from: preparation, stage backlog, signed 2026-11-02 by owner; read .farm/preparation/
      farm: pull request open 2026-11-08T17:36:18+00:00 — https://github.com/TheSTouch/Timberborn-support-auto-fill/pull/4; branch farm/3-expose-max-support-size-selector-in-the-
