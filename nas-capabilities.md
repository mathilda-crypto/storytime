# NAS capabilities

Checked against the public capability catalog (structure version 2.2.0) in the UGOS Skill Creation Tool. The parent Skill only delegates to the experts below; the experts choose their own Actions. The Action names are listed for transparency only.

| Storytime step | Expert | Catalog capability used by the expert | Effect and approval |
|---|---|---|---|
| Read settings, programme and achievement bank | `file-agent` | `ug-filesystem` (ls, cat, find) | read |
| Save an entry, settings, programme, plan | `file-agent` | `ug-filesystem` (touch, echo) | state change, approval |
| Tag entries by journey or privacy (optional) | `file-agent` | `ug-filemgr` (tag-add-file) | state change, approval |
| Copy a draft into a shared folder | `file-agent` | `ug-filesystem` (cpmv, copy) | state change, approval |
| Transcribe a voice note | `knowledge-agent` | `ug-knowledge` (audio-transcription) | read unless saving is requested |
| Read photographed handwriting | `photo-agent` | `ug-photo` (vision-ocr) | read |
| Find photos for a memory or album | `photo-agent` | `ug-photo` (search-screen, search-picture) | read |
| Create an album of confirmed photos | `photo-agent` | `ug-photo` (create-album) | state change, workflow approval |
| Talk with my diary / coach | `document-agent` | `ug-document` (qa, with citations) | read |
| Read job ad, role description, LinkedIn export | `document-agent` | `ug-document` (qa, extract) | read |
| CV, cover letter, LinkedIn and story drafts | `document-agent` | `ug-document` (writing – draft copy, original untouched) | mixed, approval |

## Needs testing on a NAS

1. Whether `ug-document` qa reads Markdown journal entries in a folder and returns sentence-level citations.
2. Voice notes in Swedish: transcription has explicit options for zh, en, de and ja; Swedish uses "other". Check accuracy.
3. Delay between a confirmed save and an entry appearing in diary answers (save verification is not index readiness).
4. Whether `ug-document` writing can save a draft into the named application folder.
5. Approval prompts: how many approvals one session needs, and whether this feels acceptable to users.
6. Whether the NAS AI chat keeps one conversation open while the user switches between Skills, and how "where was I?" behaves after switching to another Skill and back.

## Not in the catalog

Email, SMS, push notifications and scheduling; encryption; sharing with named people; calendar files; PDF layout; web access (LinkedIn, job sites). See [Limitations and roadmap](limitations-and-roadmap.md).
