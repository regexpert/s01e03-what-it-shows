**Reports covered: 374** (of the 412 in #4471)

The shared date parser reads every date month first. Tenants whose locale writes the day first get flipped dates (12 May becomes 5 December).

- Seen at all 11 tenants, in app, email and form reports, 1 April to 4 October 2026.
- Fix: parse by the tenant's locale, not month first. This is the fix already queued under #4471.
- Report ids are in `reports-4471.json` in the support kb export (tenant, channel and body decide the cause).
