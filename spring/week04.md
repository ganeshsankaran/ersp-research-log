# Spring Week 4 (April 20 - April 26)

**Goals:**
- [x] Attend weekly meeting with Aarti
- [x] Attend weekly VLab meeting
- [x] Attend weekly meeting with William and/or Prof. Bultan
- [x] Attend weekly group meeting
- [x] Evaluate “Jerry”
- [x] Migrate “Jerry” to VLab repo

**Other accomplishments:**
- Evaluated “Quacky”

**Week 4 Summary (12.5 hours):**
- Monday: Attended weekly meeting with Aarti, evaluated “Jerry” (4.5 hours)
- Tuesday: Attended weekly VLab meeting, migrated “Jerry” to VLab repo (1.5 hours)
- Wednesday: Evaluated “Quacky,” attended weekly meeting with William and/or Prof. Bultan (2 hours)
- Thursday: Evaluated “Quacky” (1 hour)
- Friday: Attended weekly group meeting, evaluated “Quacky” (3 hours)
- Sunday: Evaluated “Quacky” (0.5 hours)

**Sunday, April 26 (0.5 hours):**
- Evaluated “Quacky”
  - I ran tests on the sanitized EC2 policies

**Friday, April 24 (3 hours):**
- Attended weekly group meeting
  - We fixed all remaining discrepancies in counts
- Evaluated “Quacky”

**Thursday, April 23 (1 hour):**
- Evaluated “Quacky”
  - I noticed that the policy with IP address conditions took a long time to run. I tried to implement a new version of IP address conditions by returning lower and upper integral bounds corresponding to the bit string, instead of returning a bit string as a regular expression.
  - This idea doesn’t look like it will work because ABC doesn’t work with large numbers like Z3 and Z3 took up more memory/time when using the ints instead of the regex. 

**Wednesday, April 22 (2 hours):**
- Evaluated “Quacky”
  - I refined the use of configuration files and cleaned up the Markdown syntax used by our runners.
  - I used a Z3 implementation of a model counter to count instances satisfying the IfExists condition in a couple of policies.
- Attended weekly meeting with William and/or Prof. Bultan
  - We discussed our final discrepancies
  - We aim to fix these discrepancies by the end of the week

**Tuesday, April 21 (1.5 hours):**
- Attended weekly VLab meeting
- Migrated “Jerry” to VLab repo
  - For now, our tool is called “Quacky.” “Mark” and “Jerry” have been left behind in the ERSP repo.

**Monday, April 20 (4.5 hours):**
- Attended weekly meeting with Aarti
  - Slides can be found here.
- Evaluated “Jerry”
  - I added .exists expressions for the condition assertions
