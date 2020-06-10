# Spring Week 3 (April 13 - April 19) 

**Goals:**
- [x] Attend weekly meeting with Aarti
- [x] Attend weekly VLab meeting
- [x] Attend weekly meeting with William and/or Prof. Bultan
- [x] Attend weekly group meeting
- [x] Evaluate “Jerry”

**Other accomplishments:**
- Cleaned up “Jerry”

**Week 3 Summary (10 hours):**
- Monday: Attended weekly meeting with Aarti, evaluated “Jerry” (1.5 hours)
- Tuesday: Attended weekly VLab meeting (2 hours)
- Wednesday: Attended weekly meeting with William and/or Prof. Bultan, evaluated “Jerry” (2 hours)
- Friday: Attended weekly group meeting, cleaned up “Jerry,” evaluated “Jerry” (4.5 hours)

**Friday, April 17 (4.5 hours):**
- Attended weekly group meeting
  - We made slight fixes to our translator that made the counts line up better. See the plots below.
  - We noticed an error with “Not” conditions in “Deny” statements.
- Cleaned up “Jerry”
  - I replaced the awful nested loop with listify() calls with a single method called sanitize() that recursively “listified” a policy before it was passed into the translator
  - This made our code look slightly better and actually fixed a bug caused by a boolean as a condition value!
- Evaluated “Jerry”
  - I ran the tests again with the new version of “Jerry.” It seems that it is slower again because of our new fixes that improved accuracy/precision.

**Wednesday, April 15 (2 hours):**
- Attended weekly meeting with William and/or Prof. Bultan
  - We talked about integrating EC2 and using config files instead of command-line arguments.
- Evaluated “Jerry”
  - I scoured EC2 documentation to figure out the regular expressions we needed to support EC2 policies properly

**Tuesday, April 14 (1 hour):**
- Attended weekly VLab meeting

**Monday, April 13 (1.5 hours):**
- Attended weekly meeting with Aarti
  - Slides can be found here.
- Evaluated “Jerry”
  - I fixed the type constraints that caused iam_simplest_policy to be shown as too permissive compared to other policies (it was an outlier in our scatter plot of counts)
