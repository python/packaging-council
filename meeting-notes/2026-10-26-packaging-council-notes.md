# Python Packaging Council meeting notes (26 October 2026)

## Attendees

- Brett Cannon
- Deb Nicholson
- Henry Schreiner
- Paul Moore
- Ralf Gommers

## Discussion Notes

- Paul opinions:
  - Not too much in flight
  - PEP 771 (default extras)
      - No strong opinion, see what the community thinks
      - Look into how much impact this will have; Paul thinks it's important to think about backward compatibility and impact
      - People don't like to change stuff, don't assume they will
Wheel Variants (PEPs 817, 825, 850)
      - Mostly just Paul, disappointed by lack of conversation recently. Not enough community involvement so far
      - More breadth to the current council might help move this forward
  - Long version numbers
      - Briefly chatted on this
  - Paul never really had any say over PyPI
      - Could be tightened up a bit to be only for packages, could push for pruning there
  - "You got the vote, you get to handle the problems" :)
  - What would you like, Paul, if you had time?
      - Focus on individuals doing stuff without friction
      - PEP 723 was a great one, more of that
      - Making Python work in hostile environments (no external ports, etc.) when you need a dependency
  - We (Brett) have some (crazy, long range) plans that might help
  - We don't have people / funding to do enough in pip and our tools
      - (Paul) Funding stuff sounds hard
      - (Deb) We might be able to, we need to know what needs funding
  - Current gap: If you have more than one file but don't have a whole package, especially no PyPI access
  - Feel free to stop by office hours, Paul!

- Process PR for PEP 1:
  - Now in progress. https://github.com/python/peps/pull/5196

- Pronouncement for PEP 847:
  - Maybe try to see if there's anything we can check quickly and give feedback or ask questions, before looking at a pronouncement with the full council? Standard codes for certain failures, perhaps?
  - The two members that are most involved are absent today

- Guide update:
  - Can link to the council repo
  - Maybe make a custom 404 with a link to the homepage?
  - Summaries: remove pypa/nonpypa distinction, clean up some old projects, maybe set rules
  - Do we want a compiled tutorial page?
  - Mission statement: decide where we want to go before doing page by page (though some can be deleted sooner)

