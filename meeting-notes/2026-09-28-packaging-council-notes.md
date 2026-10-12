# Python Packaging Council meeting notes (28 September 2026)

## Attendees

- Donald Stufft
- Henry Schreiner
- Pradyun Gedam
- Ralf Gommers

## Discussion Notes

- We discussed a few governance and logistics topics.
  - We agreed to update PEP 772 so it no longer says it replaces PEP 609.
  - **Action Item:** Pradyun to make this change.
  - We'd prefer PPC members to drive our own meetings.
- We discussed how to use the [packaging-council repository](https://github.com/python/packaging-council).
  - We'll maintain a separate meeting agenda, using the repository's issue tracker as our inbox for community requests and internal tasks.
  - We'll publish meeting notes as weekly Markdown files.
  - Before making the repository public, we'll populate it with notes and some high-level issues, locking those that aren't intended for discussion.
- We spent most of the meeting discussing how to make contributions to packaging standards easier.
  - Small changes should be possible through pull requests to `packaging.python.org`, without requiring a PEP.
  - Larger changes would require a PEP.
    - We discussed separating high-level proposals from detailed specification changes, potentially using a PEP alongside a PR to the standards documentation.
    - The exact process is still to be worked out.
  - We'd like to encourage working prototypes and testing against real-world packages before approving substantial changes.
  - We'll document the updated contribution process on `packaging.python.org`, replacing or updating the existing documentation on `pypa.io`.
- We discussed improving the PEP review process.
  - We want to keep public discussions on `discuss.python.org`, but be more proactive about limiting unproductive or repetitive discussion.
  - PEP authors should be able to ask the council for help managing discussions.
  - We'd like to proactively seek feedback from maintainers of projects affected by proposed standards.
  - We discussed reducing sponsorship requirements for experienced PEP authors, possibly maintaining a list of trusted packaging contributors. We'll need to discuss this with the Steering Council.
- We briefly discussed feedback from the PPC election.
  - **Action item:** Pradyun will relay this feedback during the election retrospective with PSF staff.
