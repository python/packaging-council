# Python Packaging Council meeting notes (8 October 2026)

## Attendees

- Brett Cannon
- Deb Nicholson
- Donald Stufft
- Donghee Na
- Henry Schreiner
- Pablo Galindo Salgado
- Pradyun Gedam
- Ralf Gommers
- Savannah Ostrowski
- Thomas Wouters

## Discussion Notes

- Note taking logistics
  - The SC uses Notion for agendas, notes, and public summaries, with templates and rotating note-takers.
  - We discussed options for the PPC, including automated transcription and summaries. No decision yet on what we'll use.
- Increasing who can sponsor PEPs
  - We discussed allowing PPC members and other packaging contributors to sponsor PEPs without needing a Python core developer.
  - The SC was broadly supportive, and happy to leave the implementation details to the PPC.
  - We should have clear criteria for who gets sponsorship rights, and periodically review the list. These lists tend to grow over time, and removing people can be tricky (based on experience from other lists of trusted people like the PSRT).
  - We don't see a need to prevent core developers from sponsoring packaging PEPs.
- Decision making for PEPs that overlap packaging and CPython
  - Some topics, particularly virtual environments, don't fit neatly under either council.
  - We agreed that regular communication and "no surprises" is the right approach, rather than introducing a complicated approval process.
    - Packaging PEPs affecting CPython should involve the SC, and CPython changes affecting packaging should involve the PPC.
    - PEPs should explicitly identify who is responsible for approval.
    - We don't want to split a PEP into two just because it crosses council boundaries.
  - **Action Item:** We'll set up a shared PPC/SC channel in the SC's Discord server, which won't rotate annually.
  - There was support for a standing delegation covering virtual environments and related packaging decisions, while keeping things like `site.py` with the SC.
  - **Action item:** Pradyun to submit a PR updating the standing delegations for PEPs and virtual environments.
- Shipping a launcher via python.org
  - PPC asked whether a launcher developed by the packaging community could be distributed through <https://python.org> (motivated by not having PEP 723 (inline script metadata) support in tools distributed through python.org).
  - The SC was comfortable with this in principle.
- PPC and PyPI responsibilities
  - The PPC sees itself as responsible for packaging standards and `packaging.python.org`, working closely with PyPI and the wider ecosystem.
  - The PPC can make decisions about standards affecting PyPI, while operational responsibilities and policies remain with the PSF.
  - We briefly discussed PEP 694, which is currently delegated to Dustin Ingram, and similar delegations to PyPI administrators might make sense.
- Future meetings
  - We agreed that the PPC and SC should meet like this at least once a year.
