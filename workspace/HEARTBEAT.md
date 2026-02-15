# HEARTBEAT.md

## Daily Weather Check — Sendai
- **When:** Once per day, morning (first heartbeat after 07:00 JST)
- **How:** `curl -s "wttr.in/Sendai?format=%l:+%c+%t+%h+%w"` for quick check, full forecast with `curl -s "wttr.in/Sendai?1T"` if anything notable (rain, snow, extreme temps)
- **Action:** Send Ali a short weather summary via WhatsApp if noteworthy (rain, snow, extreme heat/cold, big temp swings). Skip if it's a boring clear day — he doesn't need "it's fine" every morning.
- **Track last check in:** `memory/heartbeat-state.json`
