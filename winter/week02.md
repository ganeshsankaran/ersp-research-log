# Winter Week 2 (January 13 - January 19)

**Goals:**
- [x] Attend weekly meeting with Aarti
- [x] Attend biweekly meeting with Prof. Mirza
- [x] Attend weekly meeting with William and/or Prof. Bultan
- [x] Attend weekly group meeting
- [x] Migrate GitHub repo to ERSP organization
- [x] Work on the translator

**Week 2 Summary (13.5 hours):**
- Tuesday: Attended meeting with Aarti; attended biweekly meeting with Prof. Mirza, Attended weekly meeting with William and/or Prof. Bultan (2.5 hours)
- Wednesday: Worked on the translator (3 hours)
- Thursday: Attended weekly group meeting; worked on translator (4 hours)
- Saturday: Worked on the translator (2 hours)
- Sunday: Worked on the translator (2 hours)

**Sunday, January 18 (2 hours):**
- Worked on the translator
 - I implemented constraints involving single ‘*’ wildcards and for NotActions and NotResources

**Saturday, January 17 (2 hours):**
- Worked on the translator
 - I created classes for Action and Resource (not Principal yet) and overloaded __str__ to provide custom SMT-LIB translations of each object of the Action, Resource, Statement, and Principal classes

**Thursday, January 16 (4 hours):**
- Attended weekly group meeting
  - We spent our meeting gauging our progress and split up tasks for implementation of the translator. Our biggest challenge seems to be implementing a parser or “walk” method that can operate on the structure of the AST, or Python dictionary.
- Worked on the translator
  - I created classes for Policy and Statement to try making the parsing easier. This may end up being a dead end if I don’t find a way to piece the objects together.

**Wednesday, January 15 (3 hours):**
- Worked on the translator
  - I experimented with a recursive policy parser and hardcoded a bunch of the strings needed to construct a SMT-LIB formula

**Tuesday, January 14 (2.5 hours):**
- Attended weekly meeting with Aarti
  - Slides can be found here.
- Attended biweekly meeting with Prof. Mirza
  - We touched base regarding the semantics of policies and reviewed the high-level translation process between JSON and SMT-LIB
- Attended weekly meeting with William and/or Prof. Bultan
  - We briefly went over determining whether two policies were equivalent or incomparable based on the outputs of sets of assertions
  - Meeting notes can be found here.
- Migrated GitHub repo to ERSP organization
