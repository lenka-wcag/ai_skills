# Weekly Briefing Routine

## Schedule
Every **Monday at 10:30am AEST**.

> Note: Claude Code's in-session cron scheduler can't persist a job indefinitely on its own — recurring jobs auto-expire after 7 days. For this to run forever, set it up as a **Trigger** in Claude Code on the web (Settings → Triggers) using the cron expression and prompt below, or re-confirm with Claude each week.

**Cron:** `30 10 * * 1` (local/AEST)

## Delivery
- Slack DM to self
- Claude push notification
- Weekly output files saved to Google Drive: WGAC/Product Brain/OUTPUTS/Day_to_Day (synced locally to laptop)
- Routine spec + reusable prompt also mirrored to Google Drive (WGAC/Product Brain/Routines), Notion (Product Brain/Routines/Day_to_day), and GitHub (this file)

## What it does
Pulls from Gmail, Google Calendar, Slack, Notion, and Google Drive to build a concise, scannable two-part briefing:

### 1. Last Week in a Nutshell
- Meetings had
- Emails sent (summarized)
- Slack communications by theme/group/people
- Activity summary (Notion, Claude, email, Slack, calendar, docs created/shared/viewed)

### 2. Week Looking Forward
- Meetings booked in (times, attendees, prep needed)
- Emails needing action / unreplied
- Slack DMs or mentions needing a reply
- To-do / action items for the coming week
- Deadlines
- Outstanding commitments to others
- Reminders
- Key task list for the week

If a section has nothing notable, it says so explicitly and includes a highlight of recent progress instead of leaving it blank.

## Reusable prompt (for the Trigger)
```
Generate my weekly briefing. Look back over the last 7 days and forward over the next 7 days using Gmail, Google Calendar, Slack, Notion, and Google Drive. Structure it as:

1. "Last Week in a Nutshell": meetings had; emails sent (summarized); Slack communications summarized by theme/group/people; an activity summary of time spent and work done (Notion, Claude, email, Slack, calendar, docs created/shared/viewed).

2. "Week Looking Forward": upcoming meetings (time, attendees, prep needed); emails needing action/unreplied; Slack DMs or mentions needing a reply; to-do/action items for the coming week; deadlines; outstanding commitments to others; reminders; a key task list for the week.

Keep it concise and scannable, sectioned with clear headers (Meetings, Actions, Reminders, Initiatives/Projects, etc). If a section has nothing notable, say so and include a highlight of recent progress instead. Send the result as a Slack DM to myself and as a Claude push notification. Save a copy of the output as a dated markdown file in WGAC/Product Brain/OUTPUTS/Day_to_Day on Google Drive.
```

## History
- **23 Jul 2026** — routine set up and first briefing generated/sent (first week on the job, so largely onboarding-focused).
- **23 Jul 2026** — output storage moved to Google Drive (WGAC/Product Brain/OUTPUTS/Day_to_Day); routine spec mirrored to Google Drive (Product Brain/Routines), Notion, and GitHub (this file).
