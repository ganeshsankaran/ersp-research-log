# Winter Week 4 (January 27 - February 2)

**Goals:**
- [x] Attend weekly meeting with Aarti
- [ ] Attend biweekly meeting with Prof. Mirza (canceled) 
- [x] Attend weekly meeting with William and/or Prof. Bultan
- [x] Attend weekly group meeting
- [x] Work on the translator

**Week 4 Summary (10 hours):**
- Tuesday: Attended weekly meeting with Aarti, attended weekly meeting with William and/or Prof. Bultan (3 hours)
- Thursday: Attended weekly group meeting, worked on the translator (4 hours)
- Saturday: Worked on the translator (3 hours)

**Saturday, February 1 (3 hours):**
- Worked on the translator
- In order to overcome the issue of accidentally declaring variables twice, I tried maintaining an unordered set of all declarations to be dumped at the top of our SMT file. I wasn’t able to get it fully working in Python yet. I created an issue on GitHub.

**Thursday, January 30 (4 hours):**
- Attended weekly group meeting
  - We worked on the translator and began implementing conditions
  - One technical issue we need to work around is the naming of variables corresponding to the conditions. In other parts of the policy, we’d only have one declaration per variable, but with conditions, we may have multiple. Naively declaring variables multiple times will cause an error in Z3.
- Worked on the translator
  - I implemented several conditions and averted a naming issue by replacing ‘:’ with ‘.’

**Tuesday, January 28 (3 hours):**
- Attended weekly meeting with Aarti
  - Slides can be found here.
- Attended weekly meeting with William and/or Prof. Bultan
  - We discussed potential bugs in Z3 or ABC and their respective workarounds
  - We talked about the efficiency of translating regular expressions into logical constraints
