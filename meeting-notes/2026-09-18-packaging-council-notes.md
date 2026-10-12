# Python Packaging Council meeting notes (18 September 2026)

## Attendees

- Brett Cannon
- Deb Nicholson
- Donald Stufft
- Henry Schreiner
- Pradyun Gedam
- Ralf Gommers

## Discussion Notes

- Greetings, pleasantries, and some non-public discussion [note taker was not sure what is OK to share publicly from this]
  - We didn't even talk about doing any sort of intro -- everyone knows everyone.
- It was almost entirely a logistics meeting.
  - How/where we'd keep track of what we need to do
    - modeling after the SC, a repository in the python/ org
      - the SC doesn't have any tooling to be shared with us, unless we count GitHub as a tool
  - How/where/how often we'd meet
    - weekly, for starters. We have a lot to talk about.
  - Who all do we need in our meetings
    - Let's have PPC + single PSF liason for now, we can invite people as needed and also set up one-offs.
  - How do we want to chat amongst ourselves?
    - Let's use Discord, at least as our backup chat channel for logistics (hey, join the meeting which is now!)
    - We'll have separate channels every year, since we would be talking about individuals at times and they might get elected in a future PPC.
  - How are we going to take notes in our meetings
    - Let's record the transcripts. We might need to redact parts of the transcript though (like personal details from today's meeting) so let's share a summary based off of it.
  - Who do we want to meet as a one-off? (at least)
    - Existing delegates, in case there's anything to handoff
    - PSF board has expressed interest
    - Python Steering Council has expressed interest
    - PSF staff (PyPI and security focus)
    - Distributors (conda, OS distros, etc)
  - We need the PSF board and PSC to update their delegations
  - How will we share notes / communicate with the wider Python community
    - We want to do a good job on this
      - At least one member likes being the note taker in meetings
      - Let's start by trying to do this async and eagerly
        - Use the next meeting as the last chance to review the notes before publication, if we haven't published already
    - Let's post on dpo, although we might want to lock the thread depending on whether we want that to be a discussion channel (or just a broadcast one)
      - Created a dpo group for moderators to be able to message us
    - Let's use the GitHub repository?
    - Office hours, although logistics TBD (We were over time already)
      - A text-only meeting, like the PSF Board office hours
        - This group is going to be accessible via text on dpo already
      - Let's try to do video calls
        - logistics TBD
  - We agreed that folks should abstain/recuse themselves from voting on PEPs/topics they're involved in (eg. Ralf and Donald for wheel variants).
  - We should all get the ability to land PRs in the peps.python.org repository
    - We'll need to figure out who to get OKs from to do this, probably the SC
  - Moving packaging.python.org out of the pypa
    - We think we should, and the python org is probably the best place? That's a future task, although let's get buy-in from active editors now.
- We briefly discussed what our priorities are.
  - (This discussion resulted in increasing the meeting frequency)
  - Are there any outstanding PEPs?
    - No, but a few are due to be submitted soon! (everyone looked at Ralf, for PEP 725/804)
  - We looked at some analysis that Pradyun did for what people voted for.
  - We talked about the standards process being a priority (it's closely related to our other topics).
  - We agreed there's a lot of things to do, and we need more time to have this conversation.
- Unrelated: We talked about making Ralf a maintainer of `packaging`, which he expressed interest in.
  - This wasn't a PPC thing, and it came up since almost all the PPC members were `packaging` maintainers already and Ralf is a pyproject-metadata maintainer already.
