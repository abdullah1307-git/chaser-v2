# Chaser v2: invoice tracker for freelancers

Built from a lo-fi prototype (Miro, 8 screens) after user interviews, context mapping and ideation.

**Problem:** Freelancers track unpaid invoices in spreadsheets, notes and folders. These go out of date when they get busy, and nothing tells them when an invoice is late.

**Design goal:** People who are owed money can see who owes what and how late it is, without remembering to update anything, and follow up on time.

## Screens (same order as the prototype)
1. Sign in (demo only, no account is created)
2. Today: what needs action, owed by client
3. Send reminder: tone (friendly, firm, final) and editable message
4. Reminder sent: log, undo, offer to turn on auto reminders
5. Auto reminders: Chaser prepares due reminders on Today
6. Add or edit invoice: auto invoice number, currency per invoice, due date worked out
7. Invoice details: partial payments, mark paid, edit, delete with undo
8. All caught up (shown on Today when nothing needs action)

## From research to decisions
- "Nothing tells me an invoice is due" -> Today screen and auto reminders
- Busy weeks break tracking -> status is calculated from dates, nothing to update
- Awkward to chase -> ready-made reminder with tone
- Partial payments, many currencies, inconsistent numbers, form keeps old values -> built in
- Heuristic review fixes: edit, undo delete, import backup, labelled buttons

## Limits
Data is saved in the browser only. Reminders open your email app or copy the text, they are not sent by a server. AI invoice reading is not built yet.

## Run / deploy
Open `index.html`. Static site: deploy on Vercel with default settings (no build step).
