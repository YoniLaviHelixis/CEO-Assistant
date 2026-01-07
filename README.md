# CEO Check-In Power Automate Flows

This repo contains two import-ready Power Automate flow definitions to run an AM check-in and PM sweep for the CEO.

## Prerequisites
- Microsoft Teams Workflows app enabled in the tenant.
- Microsoft To Do connector authorized for the account running the flow.
- Power Automate environment set to Eastern Time (US & Canada) / Eastern Standard Time.

## Files
- `flow1-ceo-checkin-am.json` — Weekday 8:45 AM check-in that captures Top 3, Inbox, and blockers.
- `flow2-ceo-sweep-pm.json` — Weekday 3:30 PM sweep that captures close/next/risks.

## How to modify the schedule or recipient
1. Open the flow JSON and adjust the `Recurrence` schedule:
   - AM flow: `hours: [8]`, `minutes: [45]`.
   - PM flow: `hours: [15]`, `minutes: [30]`.
2. Update the `Initialize_CEO_Email` action to the CEO's email address.

## Dictation tips
- In Teams desktop or mobile, tap the microphone icon in the input to dictate.
- Speak one task per line and pause between items for the best split results.
