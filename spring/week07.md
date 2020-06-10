# Spring Week 7 (May 11 - May 17) 

**Goals:**
- [x] Attend weekly meeting with Aarti
- [x] Attend weekly VLab meeting
- [x] Attend weekly meeting with William and/or Prof. Bultan
- [x] Attend weekly group meeting
- [x] Document “Quacky”
- [x] Prepare poster

**Other accomplishments:**
- Implemented feedback from FSE paper

**Week 7 Summary (12.5 hours):**
- Monday: Attended weekly meeting with Aarti (0.5 hours)
- Tuesday: Attended weekly VLab meeting (1 hour)
- Wednesday: Attended weekly meeting with William and/or Prof. Bultan, implemented feedback from FSE paper (5 hours)
- Friday: Implemented feedback from FSE paper (5 hours)
- Saturday: Prepared poster

**Saturday, May 16 (1 hour):**
- Prepared poster
  - I created new charts (box-and-whisker and bar) for our poster

**Friday, May 15 (5 hours):**
- Implemented feedback from FSE paper
  - I modified the constraints for domains to make the percentage of permissiveness estimate more accurate
  - I modified the runner to provide a percentage of permissiveness estimate
  - I tested my implementation with a simple sanity check policy and domain and then with a suite of policies and domains from Emily. The outputted percentages were around 0.5 percent to 5 percent, which seems very reasonable.
- Documented “Quacky”
- Attended weekly group meeting
- Prepared poster

**Wednesday, May 13 (5 hours):**
- Attended weekly meeting with William and/or Prof. Bultan
- Implemented feedback from FSE paper
  - I did some major refactoring to allow for a report of percentage of permissiveness
  - The percentage of permissiveness is a measure of how many requests contexts are allowed by the policy out of the total number of request contexts for a domain
  - If the domain is provided this is easy; simply create a SMT formula with the policy and domain assertions and another SMT formula with the domain assertions, and divide the former count by the latter
  - If the domain is not provided, then create a dummy domain with all ‘*’
  - In some cases, the domain size can be calculated as the product of geometric series
  - In my implementation, I assume that all condition keys and values would be specified in the domain, and that there is a one-to-one mapping of condition keys to values

**Tuesday, May 12 (1 hour):**
- Attended weekly VLab meeting

**Monday, May 11 (0.5 hour):**
- Attended weekly meeting with Aarti
  - Slides can be found here.
