# Spring Break

**Goals:**
- None in particular

**Spring Break Summary (14 hours):**
- Monday: Created “runners” to run “Mark” and “Jerry” on several test policies
- Tuesday: Worked on runners
- Wednesday: Worked on runners, worked on “Mark” and “Jerry,” tested “Mark” and “Jerry”
- Friday: Integrated type constraints for model counting

**Friday, March 27 (4 hours):**
- Integrated type constraints for model counting
  - I refactored Albert’s web scraper for AWS type and property reference to reduce unnecessary file I/O operations and to prettify the output.
  - I still need to replace the ${} identifiers with regular expressions
  - This requires us to maintain a mapping of identifiers to their corresponding regular expressions

**Wednesday, March 25 (6 hours):**
- Worked on runners
  - I finished implementing runners for Mark and Jerry on single and multiple policies
  - I added a few command-line options to make testing easier
  - I added Markdown support to create tables in our repo
- Worked on “Mark” and “Jerry”
  - I completely overhauled regular expressions for “Mark”
  - “Mark” passes more tests but runs slowly in some cases
- Tested “Mark” and “Jerry”

**Tuesday, March 24 (2 hours):**
- Worked on runners
  - I cleaned up the repo to avoid copying our source repeatedly
  - I wrote a script to migrate our changes to the appropriate directories

**Monday, March 23 (2 hours):**
- Created “runners” to run “Mark” and “Jerry” on several test policies
  - I noticed a couple of bugs in our translators, which I fixed
  - After these bug fixes, neither ABC nor Z3 reported any errors in our translation
  - Some formulas took a lot of time to solve (~5 min!) and some sat/unsat outputs did not match up with William’s outputs, which we must look into and resolve
