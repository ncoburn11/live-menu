# Weekly tasting-note sync: reading the Google Sheet

Sheet `1UVE-yAzlKXEOEK8U1_znxgEOAi7Pgcqs9pifJTkUX0Q`, tabs "FA - Tasting Notes", "SIRIUS", "Vuze - Tasting Notes".

- The UNSORTED column (E on FA/Vuze, F on SIRIUS) is long: FA runs past row 700. NEVER read a fixed range such as A1:Z200.
- Read each tab in full: first call `get_spreadsheet` for the tab's `rowCount`, then read `A1:Z<rowCount>` in chunks of at most ~400 rows until the end. Confirm the last chunk ends at the final row.
- Match every missing menu strain against BOTH the Name/Tasting Notes columns and the full UNSORTED entries ("Brand x Collaborator | Strain | Vape Cart | 1g - Type - Notes"). Search the whole UNSORTED column before concluding a note is missing.
- Never skip an item as "not in the sheet" until the full tab has been read.
