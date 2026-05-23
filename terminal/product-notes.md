# Product Notes

These are implementation/product details behind the guide.

- CoCalc terminals use xterm.js, like many modern browser terminal surfaces.
- A terminal can be anchored by a `.term` file. The containing directory
  determines the startup working directory, and the path gives collaborators
  and agents a stable identifier.
- The backend terminal service exposes session list, history, state, cwd, and
  write operations through `cocalc project terminal`.
- Multiple collaborators can attach to one live terminal stream. Shared resize,
  CPR handling, leader selection, and stale-viewer booting are part of making
  this work reliably.
- High-volume output is adaptively throttled and flow-controlled so CoCalc
  reduces message pressure without simply dropping output.
- The `open` command bridges the shell back to the CoCalc browser workspace.
