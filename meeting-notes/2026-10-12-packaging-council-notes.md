# Python Packaging Council meeting notes (12 October 2026)

## Attendees

- Donald Stufft
- Henry Schreiner
- Pradyun Gedam
- Ralf Gommers

## Discussion Notes

- We agreed that the [packaging-council repository](https://github.com/python/packaging-council) is ready to be made public!
  - The README, repository structure, initial issues, and labels are in place.
  - We’ll announce it publicly and invite people to add topics to our agenda.
    - That should be enough for now; we don’t plan to actively go looking for more issues just yet.
- We caught up on meeting notes and our review process.
  - We approved the notes from the previous two weeks, included in [PR #4](https://github.com/python/packaging-council/pull/4) alongside the initial repository setup.
  - We agreed to disable auto-merge and land [PR #5](https://github.com/python/packaging-council/pull/5), which aligns the filenames and titles with the SC’s updates.
  - We’ll keep using our shared (private) document for working notes, with its public-notes tab for reviewing drafts.
- We discussed who should be able to sponsor packaging PEPs.
  - Following our meeting with the SC, Pradyun opened [a PR updating the standing delegation](https://github.com/python/steering-council/pull/368).
    - It covers packaging PEPs and virtual environments, and would allow the PPC to approve additional packaging PEP sponsors.
  - We need a clear process for [maintaining the sponsor list](https://github.com/python/packaging-council/issues/3).
    - Our preferred approach is to add experienced authors of significant packaging PEPs, with PPC approval and some curation.
    - We also discussed removing people who become inactive in the packaging community, with three years of inactivity as a possible threshold.
    - We don’t think we need to ensure representation from particular projects in the way the PSRT does: this role doesn’t require the same immediate response.
  - We think sponsors should also get commit access to the PEPs repository.
    - Lack of access has been a source of friction, and we think granting it is relatively low stakes.
    - Maintaining the access list will take some initial work, but should settle down over time.
- We talked through what we’d want to do for our public office hours.
  - We want to try video calls, for 30 minutes every two weeks.
    - We can stay longer when needed.
    - If the first few sessions are busy or a little messy, that’s fine—and a sign people want to participate!
  - We’ll try the PyPA Discord, after testing the interface ourselves.
    - We also floated renaming it to the Python Packaging Discord.
  - The time should differ from our regular council meeting.
    - We have a candidate slot to check with Brett before settling it.
  - We’ll put the details in the repository’s README.
- We briefly discussed meeting with the PSF board.
  - The new board needs some time to settle into its roles before we arrange that.
- We reviewed feedback from the first PPC election.
  - We discussed how to encourage a broader range of candidates, including across ages, genders, and packaging projects.
    - Making the wider packaging community more welcoming matters here.
    - Ideas included first-time contributor workshops or sprint rooms at events, and exploring whether the SC’s diversity work could help.
  - Who should write election announcements?
    - Our preference is for a council member whose term continues into the next council, potentially with several members contributing.
    - The election organiser could handle this if needed.
    - We added a follow-up task to settle where announcements should go and who writes them.
  - Candidate AMAs were well received, but some candidates hadn’t known to expect them.
    - We should plan for them and tell candidates in advance next time.
    - A shared thread for questions to all candidates was suggested.
  - We kept a proposal to consider STAR voting for a future election on the to-do list; we haven’t decided to adopt it.
- We also populated our task list with upcoming work.
  - We opened [a tracking issue for moving `packaging.python.org` into the `python` GitHub organisation](https://github.com/python/packaging-council/issues/6).
    - Pradyun will look into what the move might break before proceeding.
  - We added [a review of `packaging.python.org` and](https://github.com/python/packaging-council/issues/7) [`pypa.io`](http://pypa.io) to our TODO list.
    - Update the sites to reflect the PPC’s existence,
    - then review their content, including very old pages.
  - An initial review of outstanding packaging PEPs is also “on deck”.
  - Longer-term items include making standards contributions easier, exploring how to unblock the Upload 2.0 API, and meeting with ecosystem stakeholders, including conda leadership and wheel-next.
