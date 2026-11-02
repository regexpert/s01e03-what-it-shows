**Reports covered: 5** (of the 412 in #4471)

A date lands exactly one day away from the date booked. This is not a month/day swap. It looks like a time-zone or day-boundary bug.

- R-41202: invite says Tuesday 12 May, calendar says Monday 11 May.
- R-41209: every booking in June is one day off.
- R-41236: the invite arrived before the booking was made.
- R-41344: client in Lisbon got Tuesday, client in Toronto got Monday, same meeting.
- R-41620: Tuesday 6 October showed as Monday.

The desk filed all five under the parser by tenant (`desk-notes.json`, `oneDayMove`). They need their own investigation.
