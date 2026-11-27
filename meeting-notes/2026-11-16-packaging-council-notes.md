# Python Packaging Council meeting notes (16 November 2026)

## Attendees

- Brett Cannon
- Henry Schreiner
- Pradyun Gedam
- Ralf Gommers

## Discussion Notes

- We have completed an initial review of outstanding packaging PEPs.
- We marked doing an initial review of outstanding packaging PEPs as completed.
- We briefly talked about the [Friction in packaging PEPs](https://blog.schuetze.link/friction-in-packaging-peps/) blog post.
  - We've started addressing how to make small changes to standards.
  - We also liked trying an informal "final comment period" (FCP) so people know when to raise anything that's still outstanding.
    - When a PEP is put forward for a decision, an author or a council member could post in the discussion thread with a window for last comments before we discuss it. The timing is open, and we'd be happy to follow a wider PEP process change if one comes along.
  - There are separate discussions about formally having FCP in the PEP process.
  - Markdown support for PEPs came up as a possible small improvement.
    - For now, linking to the PEP from d.p.o. removes the need for changing between formats.
  - We'll keep a closer eye on the Packaging category and help enforce the existing d.p.o. guidelines, especially when threads drift off topic. Brett can handle moderation actions when needed.
- We discussed what still needs to happen before we decide on PEP 847 (Problem Details for the Simple Repository API).
  - We will ask for a PR to bring the proposed changes into the Packaging User Guide before we accept the PEP.
- We agreed on a plan for cleaning up the Packaging User Guide's licensing.
  - We'd like the specifications and new pages to use CC0, with existing guides under CC BY-SA 3.0. As pages get rewritten, more of the Guide can move to CC0.
    - We want the material to be easy to reuse, as the source PEPs are. Keeping the existing license on older guides avoids having to seek sign-off from all their contributors up front.
  - We'll check whether the Guide maintainers agree with this approach.
    - [Public follow-up](https://github.com/pypa/packaging.python.org/issues/2187#issuecomment-6975740044)
- We agreed that adding wheel tags for `loongarch64` doesn't need a PEP. It's a CPU architecture that manylinux already supports.
  - For future CPU architecture tags, we suggested looking for broad use and support in both manylinux and `packaging`.
  - The PyPI admins decide whether PyPI accepts uploads for the architecture.
- We talked about keeping the [packaging.python.org cleanup](https://github.com/python/packaging-council/issues/8) moving.
  - Straightforward maintenance changes can be merged without additional reviews, with a second look when needed.
  - The proposed link checks would cover new links on each PR. A separate CI job would still check existing links, so an unrelated broken link can't block a contribution.
  - We were happy to try dropping the `good first issue` label and adding two prompts to the PR template -- "What motivated the change?" and "Was AI used?". We'd like to make it easier for maintainers to understand what a contribution is trying to solve.
  - The move to the `python` GitHub organisation is still pending relevant people's availability
- We're waiting for the PSF's input on the setuptools and distutils licensing question ([relevant issue](https://github.com/python/packaging-council/issues/17)).
- We discussed revisiting the implicit setuptools fallback when `build-system.requires` is absent.
  - Some projects use `pyproject.toml` for tool configuration alone. We'd like tools to be able to treat those as projects that don't need a build. We also discussed updating the Guide to help new projects choose a backend that suits them.
  - One idea is to tie the change to a future Python version so existing Python versions keep their current behaviour. We need to discuss the details further (including on the community forum).
  - We added this to our board for further discussion.
