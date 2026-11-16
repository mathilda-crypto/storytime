# Limitations and roadmap

## Known limits in version 1

- **Text conversation only.** The Skill runs inside the NAS AI chat. Choices are offered as short numbered options; the card-and-button design in the concept mockup is a target for a companion app.
- **No reminders.** Check-ins happen when the user opens Storytime. There is no email, SMS, notification or calendar invite.
- **No encryption beyond the NAS.** Entries are protected by the NAS's own accounts and folder permissions. Storytime adds no encryption.
- **Processing happens on the NAS.** The AI reads entries where the NAS models run. Which models run locally depends on the NAS setup.
- **Search delay.** A just-saved entry may not be found by diary questions at once.
- **Approvals.** Every save asks for platform approval, including "Just save this".
- **No deletion.** Users delete files with the NAS file manager.
- **Sharing is limited** to copying a file into a shared folder and creating photo albums.
- **No web access.** LinkedIn and job ads arrive as pasted text or saved files.
- **One experiment at a time.** By design.
- **No always-visible chat window.** Storytime runs inside the NAS AI chat; a floating or always-on window is part of the NAS interface, or of a future companion app. "Menu" and "where was I?" let the user move around and resume from the saved programme record.

## Roadmap

| Capability | Development needed |
|---|---|
| Talk with my diary at scale | Durable index of entries, date and topic search, answers linked to originals, correction history |
| Pictures, audio, notes and films | Recording in the app, organisation per entry, accessible playback |
| Mood and habit tracking | Optional check-ins, history, user-defined measures, review screens |
| Prompts by email, SMS, notification or calendar | Messaging and calendar integrations, quiet hours, prompts that never include entry text |
| Offline writing | Local storage, sync, conflict handling, clear offline indicators. Offline writing and offline AI are separate capabilities |
| Encrypted private journal | A defined encryption model, key management, recovery, backups, deletion and security testing. Early decision: where may AI read the journal? If an entry is processed, it must be readable at that point |
| iPad handwriting | Notebook imports or device integration, handwriting recognition, keeping originals |
| Calendars and sharing | Export tools, recipient controls, previews, sharing of selected content only |
| Family books and creative products | Selection, editing, layout, export, preservation of original material |
| Job and calendar connections | Account integrations, permissions, clear controls over external actions |
| Companion app | The mockup's screens: settings, programme map, cards and buttons |
| Food tracking and recipes | A later journey |

## Test plan for a NAS (finalist round)

Core test 1 – Write and ask: save a typed entry and a Swedish voice note, then ask "When did I first write about the interview?" Expect citations with file path and written date, and a clear note when no event date exists.

Core test 2 – Application kit: put a sample job ad PDF and role description in an application folder; build matches against a three-item achievement bank; generate a CV draft. Expect every requirement traced to its source, gaps kept in brackets, and the draft saved as a new copy.

Edge case – Just saved, not yet searchable, plus a vault entry: save an entry and ask about it immediately; save a vault entry and ask a diary question. Expect the new entry to be read by exact path, and the vault never to be cited.
