# Winter Week 8 (February 24 - March 1)

**Goals:**
- [x] Attend weekly meeting with Aarti
- [ ] Attend biweekly meeting with Prof. Mirza (changed to individual meeting)
- [x] Attend weekly meeting with William and/or Prof. Bultan
- [x] Attend weekly group meeting
- [x] Work on “Mark” and “Jerry”

**Other accomplishments:**
- Test “Mark” and “Jerry”

**Week 8 Summary (9.5 hours):**
- Tuesday: Attended weekly meeting with Aarti, attended weekly meeting with William and/or Prof. Bultan, worked on “Jerry” (5 hours)
- Wednesday: Worked on “Mark” and “Jerry” (1 hour)
- Thursday: Attended weekly group meeting (2 hours)
- Friday: Tested “Mark” and “Jerry” (1 hour)
- Saturday: Tested “Mark” and “Jerry” (0.5 hours)

**Saturday, February 29 (0.5 hours):**
- Tested “Mark” and “Jerry”
  - I wrote policies that test almost all conditions

**Friday, February 28 (1 hour):**
- Tested “Mark” and “Jerry” (1 hour)
  - I created extreme policies (ab)using wildcards. 
  - I fixed small bugs in interpreting wildcards and “Not” elements

Thursday, February 27 (2 hours):
Attended weekly group meeting
We used ABC to count models satisfying formulas produced by “Jerry”
We fixed bugs and finally got a correct model count for a test policy and corresponding domain

**Wednesday, February 26 (1 hour):**
- Worked on “Mark”
  - I incorporated the condition domain
- Worked on “Jerry”
  - I incorporated the condition domain
  - I removed “header” vs “body” distinctions for many functions because we would no longer need complex declarations for regular expressions

**Tuesday, February 25 (5 hours):**
- Attended weekly meeting with Aarti
  - Slides can be found here.
- Attended weekly meeting with William and/or Prof. Bultan
  - Meeting notes can be found here.
- Worked on “Jerry”
  - Albert and I implemented the logic to translate regular expressions into the Perl-like syntax we went over during our meeting with William and Prof. Bultan. 
  - We reintroduced action domain assertions.
  - We reintroduced conditions from the policy. It looks like we still have to use up variables for condition keys since they are necessary for proper counting.
