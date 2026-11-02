**Reports covered: 33** (of the 412 in #4471)

The booking-v3 form prints `MM/DD/YYYY` under its date field. People at day-first tenants (alder.physio de-DE, copper.studio es-ES, pale.harbour pt-PT) type what the hint tells them, month first, and the form reads it their way. This is a different bug from the parser: fixing the parser does not fix it.

- Form reports only. 17 April to 22 September 2026.
- Intake tagged 15 of the 33 as `parser` because it guessed from the browser.
- Fix: print the tenant's own order in the hint, or make the form read what it prints.
