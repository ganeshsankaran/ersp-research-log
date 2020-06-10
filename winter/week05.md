# Winter Week 5 (February 3 - February 9)

**Goals:**
- [x] Attend weekly meeting with Aarti
- [x] Attend weekly meeting with William and/or Prof. Bultan
- [x] Attend weekly group meeting
- [x] Work on the translator
- [x] Incorporate domain information into SMT formula

**Week 5 Summary (7 hours):**
- Tuesday: Attended weekly meeting with Aarti, attended weekly meeting with William and/or Prof. Bultan (3 hours)
- Wednesday: Worked on the translator (1 hour)
- Thursday: Attended weekly group meeting (2 hours)

**Thursday, February 6 (2 hour):**
- Attended weekly group meeting
- Incorporated domain information into SMT formula
  - Using Emily’s action scraper, we were able to add assertions that ensured that the actions were valid. This seemed to have added runtime, but we need to test this because right now, this is the only viable option.
  - I’m thinking of creating a “domain.json” file that contains all the valid IAM resources and variables

**Wednesday, February 5 (1 hour):**
- Worked on the translator
  - I rewrote the translation logic for IgnoreCase and IpAddress conditions
  - I wrote two versions of translations for IpAddress conditions, one of which looked cleaner but ran much slower, causing a timeout on Z3 Rise4Fun

**Tuesday, February 4 (4 hours):**
- Attended weekly meeting with Aarti
  - Slides can be found here.
- Attended weekly meeting with William and/or Prof. Bultan
  - We discussed differential analysis (relative permissiveness checking), how to set up the SMT formulas to perform differential analysis, and the practicality of differential analysis for testers (us) and users.
  - We brainstormed logical constraints to encode the domain into the SMT formula
  - We constructed logical constraints for “ignore case” conditions.
  - We proposed methods of testing our tool
  - William and Prof. Bultan mentioned the possibility of Z3 timing out if the formulas became too complex
  - William mentioned the possibility of ABC running out of memory if dates were interpreted as large integers.
- Worked on the translator
  - I was able to prevent duplicate declarations using a set of declarations. I plan on moving all header elements to this set to keep everything in one place.
  - I created cases to handle canonical, federated, and service users for Principals.
  - A potential roadblock is ‘:’ characters in AWS variables that may interfere with the way my translator splits the strings. I created an issue on GitHub.
