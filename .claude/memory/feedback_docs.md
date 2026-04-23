---
name: Keep docs in sync after feature changes
description: After significant UI or feature changes, proactively update README and check architecture diagram — don't wait to be asked
type: feedback
originSessionId: 93f74eab-0e85-4868-9ad0-206053d29e9d
---
After any significant feature change, always proactively:
1. Update the README Features section to reflect the new state
2. Check if the architecture diagram (architecture.html) needs updating — it covers data flow, not UI, so it only changes when storage or sync mechanisms change, not for UI features

**Why:** User had to ask explicitly after every change. This should be automatic.

**How to apply:** At the end of any session where features changed, update README and push it along with the feature commit (or as a follow-up). No need to ask.
