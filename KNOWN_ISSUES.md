# Known issues and validation limits

- Axe and Cross share graphics tiles. If an opposite-weapon pickup occurs while
  one is flying, pickup/HUD art can briefly retain the outgoing projectile's
  silhouette until cleanup. The projectile and selected weapon remain distinct.
- Cold-boot after changing versions. Old emulator states may resume incompatible
  custom code or graphics data, especially states saved inside the practice menu.
- BGB 1.6.6 validation and stream playtesting do not establish complete-game,
  every-frame or MiSTer/hardware correctness.
- Full natural-reference collision-cache audits remain pending for the Cloud,
  Crystal, Rock, Dracula 1 boss approaches and Final entrance. Existing testing
  covers their preset loads, but the full reference comparison is not claimed.
- The coordinate display can be harder to read over busy backgrounds.
- The Ghost Rope bug from alpha13/14 was fixed in alpha15. It remains in the
  changelog as historical evidence, not a demonstrated original-game glitch.

For reports, include alpha17, emulator/core version, US/JP weapon rules,
starting preset or normal route, expected/actual behavior and minimal inputs.
Screenshots/video are welcome. **Do not upload ROM files or save states** to
public issues; describe the state/setup instead.
