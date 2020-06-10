# Winter Week 1 (January 6 - January 12)

**Goals:**
- [x] Attend weekly meeting with Aarti
- [x] Attend weekly group meeting
- [x] Set up meetings with William and Prof. Bultan
- [x] Revise timeline for winter and spring quarters
- [x] Set up repository on GitHub
- [x] Analyze SMT-LIB translations of policies

**Week 1 Summary (4.5 hours):**
- Tuesday: Attended meeting with Aarti; set up meetings with William and Prof. Bultan (1.5 hours)
- Wednesday: Filled out reflection (0.25 hours)
- Thursday: Attended weekly group meeting; revised timeline for winter and spring quarters (2 hours)
- Sunday: Analyzed SMT-LIB translations of policies

**Sunday, January 12 (1 hour):**
- Analyzed SMT-LIB translations of policies
  - I looked at the numeric-equivalent policy and its corresponding SMT-LIB translation, paying attention to how the conditions were constructed and how p0 and p1 were compared in order to deem that the policies were “equivalent.”
  - I understand why the output of the SMT solver was unsat but I believe that the equivalence is determined by Zelkova and not the SMT solver
  - This means that we have to figure this out when working on quantifying the permissiveness of policies.

**Thursday, January 9 (2 hours):**
- Set up repository on GitHub
- Attended weekly group meeting
  - We manually translated each line of a policy into SMT-LIB so that we could figure out how to implement such a translation in our code
  - We noticed a couple of potential roadblocks going forward, such as identifying valid principals/actions/resources in a namespace as well as implementing conditions. I’m worried that the latter may delay our timeline significantly because we may not be able to translate conditions requiring the use of Z3 Automata.
  - Revised timeline for winter and spring quarters
  - We need to account for conditions, which may take up some time to do

**Tuesday, January 7 (1.5 hours):**
- Attended meeting with Aarti
  - Aarti gave us a high-level overview of the logistics for Winter quarter
- Set up meetings with William and Prof. Bultan
  - We reached out to Prof. Bultan regarding his availability. He mentioned that he would try joining our meetings with William as frequently as possible, but we may want to mention this to Aarti in case we can’t meet biweekly on average
