# TOOLS.md - Local Notes

Skills define *how* tools work. This file is for *your* specifics — the stuff that's unique to your setup.

### Google Calendar
- **Account:** ali.najaf@gmail.com
- **Calendars to check (always query all three):**
  - `primary` — personal
  - `najaf.ali@givery.co.jp` — Givery (work)
  - `ali@archpt.io` — Arch PT (freelance)
- **Always prefix event titles with a relevant emoji** (e.g. 🪪 Apply for My Number Card, 🏥 Doctor Appointment, 💼 Meeting with Simon)

### Webchat Dashboard & TUI
- **Read/tool output is not visible** in either the webchat dashboard or the TUI — Ali can't see file contents from `read` calls
- When Ali asks to see file contents, **paste the text directly into the chat message** so it's visible

### Japanese SHIFT-JIS Websites
- `web_fetch` can return garbled text (mojibake) for SHIFT-JIS encoded pages
- Use curl + iconv instead: `curl -s "URL" | iconv -f SHIFT-JIS -t UTF-8`
- Common on older Japanese sites (check for `charset=Shift_JIS` in meta tags)

### Viator Supplier Portal
- **URL:** https://supplier.viator.com
- **Username:** ali.najaf+jp@gmail.com
- **Password:** _jul13twh1sk3y

### BJJ - 草柔会仙台 (Soujiukai Sendai)
- **Website:** https://soujiukai.jimdofree.com/
- **Affiliation:** IBJJF + JBJJF, 草柔会アソシエーション本部道場
- **Instructor:** Black belt 3rd dan (certified by Carlos Gracie Jr)
- **Email:** soujiukai_cocorogym@yahoo.co.jp

**Fees:**
- ¥5,000/mo — Regular member
- ¥4,000/mo — Women/Students/Kids regular
- ¥3,000/mo — Weekend only (Sat/Sun)
- ¥2,000/mo — Women/Students/Kids weekend only

**Schedule:**
| Day | Location | Time | Class |
|-----|----------|------|-------|
| Mon | 本部道場 | 20:00-22:00 | 一般 |
| Tue | 本部道場 | 20:00-22:00 | 一般 |
| Wed | 宮城県武道館支部 | 19:00-20:30 | 一般 |
| Thu | 本部道場 | 20:00-22:00 | 一般 |
| Fri | 本部道場 | 20:00-22:00 | 一般 |
| Sat | 仙台市武道館支部 | 10:00-11:30 | 一般 |
| Sat | 本部道場 | 20:00-21:30 | スパーリング + ノーギ |
| Sun | 本部道場 | 10:00-11:00 | 45歳以上限定 |
| Sun | 多賀城支部 | 14:00-16:30 | 一般 (キッズ 14:30-) |

## What Goes Here

Things like:
- Camera names and locations
- SSH hosts and aliases  
- Preferred voices for TTS
- Speaker/room names
- Device nicknames
- Anything environment-specific

### Obsidian Vault
- **ali-vault** → `/Users/najafali/Desktop/ali-vault` (primary, ~2310 notes, git-tracked)
- Mostly flat structure, daily notes, people notes, project notes
- Also has: Givery management vault, najafali-static vault

## Why Separate?

Skills are shared. Your setup is yours. Keeping them apart means you can update skills without losing your notes, and share skills without leaking your infrastructure.

---

Add whatever helps you do your job. This is your cheat sheet.
