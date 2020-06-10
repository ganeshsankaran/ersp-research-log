# Spring Week 2 (April 6 - April 12)

**Goals:**
- [x] Attend weekly meeting with Aarti
- [x] Attend one-on-one meeting with Prof. Mirza
- [x] Attend weekly VLab meeting
- [x] Attend weekly meeting with William and/or Prof. Bultan
- [x] Attend weekly group meeting
- [x] Evaluate “Mark” and “Jerry”

**Other accomplishments:**
- Consolidate logic between “Mark” and “Jerry”
- Integrate better type constraints

**Week 2 Summary (9.5 hours):**
- Monday: Attended weekly meeting with Aarti, evaluated “Mark” and “Jerry”, consolidated logic between “Mark” and “Jerry” (3.5 hours)
- Tuesday: Attended weekly VLab meeting (1 hour)
- Wednesday: Attended weekly meeting with William and/or Prof. Bultan, integrated better type constraints (2.5 hours)
- Friday: Attended one-on-one meeting with Prof. Mirza, attended weekly group meeting (2.5 hours)

**Friday, April 10 (3.5 hours):**
- Attended one-on-one meeting with Prof. Mirza
- Attended weekly group meeting
  - We ran into roadblocks due to ABC’s lack of support for re.loop operations and the fact that the latest version of ABC wasn’t installed on Tuba

**Wednesday, April 8 (2.5 hours):**
- Attended weekly meeting with William and/or Prof. Bultan
- Integrated better type constraints
  - I rewrote the web scraper to map each resource type to all the actions that act on it. This makes it easier to write assertions where one big regex for the resource type is mapped to a bunch of short action strings rather than the other way around
  - Solving time plummeted in many cases

**Tuesday, April 7 (1 hour):**
- Attended weekly VLab meeting

**Monday, April 6 (3.5 hours):**
- Attended weekly meeting with Aarti
  - We just touched base regarding Spring quarter objectives and shared our high-level progress and revised timeline.
- Evaluated “Mark” and “Jerry”
  - I fixed the bug where an action namespace of ‘*’ would crash our translator. My solution was to mark each namespace as valid or not; for example, we can mark “s3” and “iam” as valid namespaces so that if ‘*’ shows up in our action namespace, we know to use those namespaces only.
  - The benefit of using no constraints is quick results, but the drawback is inaccuracy in counting. For iam_simplest_policy, adding no constraints makes the counting process very fast
  - The benefit of using constraints for all namespaces is precise counts, but the drawback is that it takes an eternity to count.
  - The benefit of using limited constraints is getting somewhat quick and precise results, so I see it as a good compromise.
- Consolidated logic between “Mark” and “Jerry”
  - Due to poor performance of ABC with many variables (actionNamespace and actionName vs action) and the now similar regular expressions, it made sense to consolidate the logic into “Jerry”
  - I implemented a flag that toggles SMT-LIB syntax in case we want to use off-the-shelf SMT solvers to solve the formulas. 
