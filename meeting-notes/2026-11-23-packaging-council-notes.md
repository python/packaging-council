# Python Packaging Council meeting notes (23 November 2026)

## Attendees

- Brett Cannon
- Donald Stufft
- Henry Schreiner
- Pradyun Gedam
- Ralf Gommers

## Discussion Notes

- We agreed to accept [PEP 847 (Problem Details for the Simple Repository API)](https://peps.python.org/pep-0847/).
  - We'll merge the packaging.python.org PR first.
  - We'll consider it Final once at least one client and one server implement it.
- We discussed [PEP 832 (Virtual environment discovery)](https://github.com/python/packaging-council/issues/19#issuecomment-7110780351) and deferred a decision to next week.
- We need to follow up with the PSF about the setuptools/distutils license situation.
- We discussed the remaining questions in the [initial Packaging User Guide cleanup](https://github.com/python/packaging-council/issues/8).
  - We'd like installer tabs along the lines of the existing build backend tabs. For imperative installs, that could mean adding `uv pip` alongside `pip` in the existing tutorials.
  - We'd like to eventually have a high-level page that shows the same basic steps across workflow tools (such as uv, Hatch, PDM, and Poetry) -- starting a project, adding dependencies, installing and running the project.
    - The tabs should make it easy to follow along with a widely used, actively maintained tool. Readers can go to that tool's own docs for configuration and more advanced options.
    - We also discussed documenting how to create and install from a `pylock.toml`, including how tools with their own lock formats can export one.
  - We'll drop or generalize setuptools guides -- most of the pages we have in the packaging guide are old and should just be dropped.
- We marked our discussion of [Friction in packaging PEPs](https://blog.schuetze.link/friction-in-packaging-peps/) as done after covering it last week.
- We followed up on [PEP 766 (Explicit Priority Choices Among Multiple Indexes)](https://peps.python.org/pep-0766/) after talking with Mike Fiedler at office hours.
  - The PEP is informational and gives us vocabulary for talking about how installers choose among indexes. We discussed whether common behavior across installers would call for a standard, and what we could do to improve pip's behavior in the meantime.
  - We talked through three ways installers could choose among indexes.
    - Choose the best version across all indexes.
    - Stop at the first index that has the package.
    - Continue until an index has a compatible candidate.
  - Index priority can reduce dependency confusion risk, though ordering alone cannot guarantee that a package comes from its intended source. Falling back can also be useful when a specialist index only has some builds.
  - Ralf will ask Mike Fiedler if he'd like to take over and finish the PEP. We discussed whether it could recommend a safer default.
  - Pradyun will talk to pip maintainers for a rough estimate of the work involved in adding index priority, so we can explore funding it. The exact behavior and rollout are still open.
- We briefly talked about future Packaging Summits and whether a sprint could help maintainers of different tools work together in person.
  - Attaching it to a conference such as PyCon US or EuroPython would make it easier to organize. We left the location, frequency, and travel expectations for another discussion.
