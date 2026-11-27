# Python Packaging Council meeting notes (2 November 2026)

## Attendees

- Brett Cannon
- Deb Nicholson
- Henry Schreiner
- Ralf Gommers

## Discussion Notes

- We agreed to tidy up the election discussions on d.p.o.
  - Brett will rename the nomination subcategory to Packaging Council, add an AMA tag to the candidate posts, and close the threads.
  - Would unlisting the threads make them less prominent in search while leaving the links working? Brett will check.
  - We’ll talk about election communication when more of us are there.
- We merged the [PR describing the current standards process](https://github.com/python/packaging-council/pull/18).
  - We’d still like to improve the process. We talked about how to distinguish editorial fixes, small changes to the spec, and changes that need a PEP.
    - Typo fixes and wording changes that preserve the meaning can go straight in without council approval.
  - We’ll review the remaining small spec edits in the Packaging User Guide repo offline or next time.
- We discussed the [setuptools and distutils licensing issue](https://github.com/python/packaging-council/issues/17).
  - Does code taken from CPython need to retain the PSF license? Deb has asked PSF legal and will report back.
  - We agreed that setuptools’ metadata should follow the current spec. Ralf has acknowledged the issue on GitHub and will draft our reply on that part.
    - A license expression has to cover everything in the distribution, including vendored code. Setuptools can also leave the field out.
  - How should projects say what license applies to their own code and contributions? [PEP 639](https://peps.python.org/pep-0639/) gives us a way to describe the licenses of everything they ship.
    - Could we add a field through a PR? We also discussed doing a PEP, given the different ideas about which fields to add. A new core metadata version would also need support from tools.
    - We’ll come back to this with more of the council around.
- We came back to [PEP 847 (Problem Details for the Simple Repository API)](https://peps.python.org/pep-0847/) after more feedback from index implementers.
  - How much should servers agree on which error to return when several apply? We talked about leaving that choice to servers while giving users better error messages.
    - Some shared error types or guidelines could still be useful, either in this PEP or later.
  - We’ll give the discussion another week and get input from the council members who were away. We could vote asynchronously once things settle down.
- We also discussed [PEP 832 (Virtual environment discovery)](https://peps.python.org/pep-0832/).
  - We liked that it stays close to what tools already do. It would standardize the `.venv` convention and add a redirect file for a preferred environment elsewhere. Support would be optional.
    - Handy when a project has several environments (e.g. with Nox or tox) and a tool needs to know which one to use.
  - Hatch’s feedback called for a broader solution for multiple environments.
    - We think there’s room for both, and there’s still interest in a broader protocol for managing environments.
  - We’ll keep it on the agenda and get input from the council members who were away. The PEP’s author will sit out the vote.
- We continued [reviewing packaging.python.org and pypa.io](https://github.com/python/packaging-council/issues/7).
  - We’ve been cleaning up the Packaging User Guide. We’d like to clear out more old material before adding a council page.
    - Ralf will update the standards-process links to point to the council repo.
  - Some of pypa.io is out of date too. Could it just describe PyPA and link to its projects? We’d need to talk with PyPA about that.
  - We’ll follow up on [moving the guide’s repo to the python organisation](https://github.com/python/packaging-council/issues/6) and make sure someone’s around to handle deployment hiccups.
- Do we want packaging standards to support cross-compilation better? Yes!
  - We’d like a standard way to ask for a build for a target platform. Right now the settings depend on the backend and package.
    - cibuildwheel already has several workarounds. Distro packaging and WASI wheels could use better support too.
  - A couple of potential PEP authors reached out, and Henry will talk with them later today.
