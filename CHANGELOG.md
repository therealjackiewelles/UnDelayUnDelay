# UnDelayUnDelay changelog

## v0.1.1

- Fixed: the update check could never reach GitHub — the app's sandbox was
  missing the outgoing-network permission, so every connection was silently
  blocked. Update checks now work.

## v0.1.0

First release.

- The card: enter the temperature and humidity the PA was timed at, and what
  they are now — get the speed-of-sound change and the delay drift.
- Drift shown in milliseconds and samples (44.1 / 48 / 96 kHz).
- Reference input takes your original delay (ms) or throw distance (m).
- °C / °F toggle; everything you type survives a relaunch.
- Pin button keeps the card floating above other windows.
- Checks the public repo for updates on launch and daily, with
  download-and-install — same mechanism as Mping.
- Speed of sound computed with the Cramer formula (temperature, humidity,
  standard pressure).
