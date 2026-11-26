# Structure of uae-abu-dhabi-law

The law of the Emirate of Abu Dhabi, including Abu Dhabi Global Market (ADGM). Folder names are in Arabic; under them,
courts that publish in English keep their English names. Each record is one commit, dated 12:00 UAE time on its day
(for a judgment, the day it was given). `git log --follow <file>` gives a text's history.

| Folder | What it holds | Path pattern |
| --- | --- | --- |
| `المحاكم/adgm-courts/` | judgments of the ADGM Courts, as the court publishes them (English) | `المحاكم/adgm-courts/<court-of-first-instance|court-of-appeal>/<year>/<adgmcfi|adgmca>-NNNN.md` (the neutral citation) |
| `data/`, `tools/` | tables and scripts about the record | |

Every commit carries `Kind:`, `In-force:` (the day) and `In-force-basis:` (where the day comes from: the judgment date
in the ADGM Courts judgments list). Party names are never used in paths or commit subjects; the text is as the court
published it, anonymised where the court anonymised it.
