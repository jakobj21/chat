---
name: no-instagram-handle-on-exports
description: "Never print an @-handle or account name on any Instagram export canvas — Jakob does not want handles, ever."
metadata: 
  node_type: memory
  type: feedback
  originSessionId: 7897c379-f61d-408b-b146-d57480abb8df
  modified: 2026-07-28T18:31:01.922Z
---

Never put an Instagram handle / @-name on an exported canvas (Reel background,
Story background, post overlay, profile pic — anything). Jakob said "i dont
want the handles ever" after being asked to fill in a `HANDLE` placeholder.

**Why:** Instagram already shows the posting account on every Reel and Story,
so printing it again is redundant noise on a deliberately minimal black layout.
It is a standing preference, not a one-off for a single video.

**How to apply:** Do not add a `HANDLE` constant or an @-line to any new
background generator in `Circuit_Animations/instagram/`. A plain CTA line like
"Follow for more circuit animations" is fine — the objection is to the @-name
specifically. If an existing script grows one, strip it and rebalance the
bottom band rather than leaving a gap. See [[circuit-animations-export-pipeline]].
