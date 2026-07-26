---
name: Roblox Security Checklist
description: Use before shipping systems that touch remotes, data, rewards, or permissions.
---

# Roblox Security Checklist

- Every remote input is validated.
- The server owns rewards, currency, and progress.
- There are no unsafe dynamic require paths.
- Rate limits exist for repeated requests.
- Save data is versioned and validated.
- Secrets are not exposed to the client.
- Abuse paths were tested.
