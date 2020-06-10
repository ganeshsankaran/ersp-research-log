# Winter Week 7 (February 17 - February 23)

**Goals:**
- [ ] Attend weekly meeting with Aarti (cancelled)
- [x] Attend weekly meeting with William and/or Prof. Bultan
- [x] Attend weekly group meeting
- [x] Work on the translator (“Mark”)
- [x] Work on the ABC version of the translator (“Jerry”)

**Week 7 Summary (7 hours):**
- Tuesday: Attended weekly meeting with Aarti, attended biweekly meeting with Prof. Mirza attended weekly meeting with William and/or Prof. Bultan (4 hours)
- Thursday: Attended weekly group meeting (2 hours)
- Friday: Worked on the translator (1 hour)

**Friday, February 21 (1 hour):**
- Worked on the ABC version of the translator (“Jerry”)
  - I added an argument parser to make it easier for users to specify whether they want to compare two policies, and if so, upload those two policies. I think that this is easier for users since they won’t manually want to put policies together into a JSON file.

**Thursday, February 20 (2 hours):**
- Attended weekly group meeting
  - We began implementing the first iteration of a stripped-down translator specifically for ABC
  - We incorporated pairwise comparisons of policies to check relative permissiveness
  - We need to find documentation for regular expressions so that we can translate them into the form ABC likes in its input language

**Tuesday, February 18 (4 hours):**
- Attended weekly meeting with William and/or Prof. Bultan
  - We discussed a potential limitation of plugging in our “generic” SMT formulas into ABC. This could become a substantial roadblock
  - On the bad side, we need to significantly cut down on the number of variables ABC deals with (action vs actionName and actionNamespace). This means that our way of translating regular expressions will significantly hinder the performance of ABC
  - On the good side, we can pass regular expressions into ABC with special characters and ABC will handle the details of constructing automata and such
- Worked on the translator (“Mark”)
  - I added functionality to handle multiple condition keys within a single condition operator
  - I fixed a bug translating regular expressions where regex of the form ‘b*b’ would not be translated into the appropriate assertions
  - I integrated Albert’s smart domain translator in order to construct better domains without spelling everything out for the translator
