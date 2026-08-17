# Daily Office Reader

A phone-friendly Daily Office without Leo recordings. Psalms and lessons are linked to the [Berean Standard Bible on Bible Study Tools](https://www.biblestudytools.com/bsb/), where you can read the chapter and use their audio player.

This is a sibling of [daily-office](https://github.com/mohuddle/daily-office), the same office with locally generated Qwen3-TTS voice. Keep that repo if you want the spoken office at home. Use this one if you want a light app that only points to the day’s readings.

## What this is

- **Morning / Evening** — psalms and lessons from *Daily Readings for the Christian Year* (The Trinity Mission)
- **Midday** — fixed Monday–Saturday cycle from the Trinity Mission midday card
- **Compline** — short weekly bedtime lessons
- **Lessons** — each reading is a link, in the same spirit as [Daily Office For All](https://dailyofficeforall.com/morning-prayer.html). Example: [Psalm 81 (BSB)](https://www.biblestudytools.com/bsb/psalms/81.html)
- **Daily confession** — Westminster in the morning; Heidelberg then Belgic cycling in the evening; a Confessional Echo when a lesson overlaps the Reformed Dogmatika plan
- **No Leo audio**, no weekly recording job, no MP3s

v1 does **not** include full office prayers, canticles, creed, or collects.

## Prayer times (America/Chicago)

| Office   | Time  |
|----------|-------|
| Morning  | 07:30 |
| Midday   | 11:30 |
| Evening  | 17:30 |
| Compline | 22:00 |

## Run the PWA

From the repo root:

```bash
python3 scripts/serve_lan.py --host 0.0.0.0 --ports 8766
```

Then open http://127.0.0.1:8766/

To keep it running on a Windows 11 PC after reboots, see [WINDOWS.md](WINDOWS.md). You do not need Grok Build or an xAI key.

Use port **8766** so it can sit beside the voiced Daily Office on 8765.

## Credits and inspiration

This is a small personal Daily Office. It is not affiliated with the projects below.

- [The Trinity Mission](https://thetrinitymission.org/) — morning, evening, and midday lessons
- [Daily Office 2019](https://www.dailyoffice2019.com/)
- [Daily Office For All](https://dailyofficeforall.com/) — linked lessons and a simple reading layout
- [Bible Study Tools](https://www.biblestudytools.com/bsb/) — BSB chapter pages and their audio player
- [Westminster Daily](https://reformedconfessions.com/westminster-daily/reading-plan)
- [Reformed Dogmatika Bible Reading Plan](https://reformeddogmatika.com/reformed-bible-reading-plan/)

Scripture text of the opening sentences and the linked chapters is the [Berean Standard Bible](https://bereanbible.com/).
