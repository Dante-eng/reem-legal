# Reem – Privacy Policy

_Last updated: 2026-09-30_

Reem ("the bot") is a Discord bot with an optional web dashboard. This policy explains what it stores, why, and how to have it deleted.

## What Reem stores

- Server, channel, role and user IDs needed to run the features a server has enabled.
- Per-server settings configured in the dashboard or with commands.
- Moderation cases (target, moderator, reason, time), XP and level counters, giveaway entries, ticket records, starboard references, polls, suggestions, birthdays (month and day only), tags and creator-notification subscriptions.
- Ticket transcripts are generated when a ticket is closed and sent to the log channel the server chose and to the ticket opener. They are not kept by the bot.

## Message content

Reem reads message content only to run features a server enables (automod, leveling, and the optional AI assistant). Message content is not stored, except what a ticket transcript contains at the moment it is generated.

For the analytics tab the bot counts messages, joins, leaves and opened tickets per server per day (numbers only, never who or what), kept for 400 days.

## Music

When a member uses `/play`, the text they type or the link they paste is sent to a music server (Lavalink) that looks it up on YouTube. Reem does not store search text or listening history. The current queue exists only in the bot's memory while it is playing.

## AI assistant (optional)

If a server administrator enables the AI assistant, messages that members address to it (by mention or reply, or every message in channels the administrator selects), the member's display name, the server name, and the administrator's persona and knowledge-base text are sent to Anthropic's API to generate a reply. The last few exchanges in that channel are kept in temporary memory for 30 minutes, together with the passages of the administrator's uploaded documents that match the question.

By default conversations are not stored; only usage counters (number of answers, tokens, thumbs-up/down feedback) are kept per server per month. Administrators can opt in to a 30-day log of questions and answers, and to AI summaries of closed tickets (which sends that ticket's messages to Anthropic). Administrators are responsible for telling their members which of these are active.

## Dashboard login

Logging in uses Discord OAuth2 with the `identify` and `guilds` scopes. Access tokens are discarded after login. A session records your user ID, display name, avatar and the servers you can manage, and expires after 12 hours.

## Retention and deletion

- If the bot is removed from a server, that server's data is deleted automatically after 7 days (re-inviting the bot within that time keeps it).
- Server administrators can delete all of a server's data at any time from the dashboard (**Data & privacy**).
- Anyone can erase their own data from the dashboard (**Your data** on the server list): levels and giveaway entries are deleted, and moderation and ticket records that other people rely on are anonymised.
- Housekeeping deletes finished background jobs after a day, failed ones after 30 days, processed payment-webhook identifiers after 90 days, and dashboard activity logs after a year.

## Children

Reem follows Discord's minimum age requirements and does not knowingly collect data from anyone below them.

## Changes

This policy may be updated; the date above shows the latest version.
