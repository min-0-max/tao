---
"tao": patch
---

On macOS, `EventLoopExtMacOS::set_activate_ignoring_other_apps(false)` no longer calls `activateIgnoringOtherApps(false)` at launch, which activated the application when no other application was active. The activation is left to Launch Services, so a background launch stays in the background.
