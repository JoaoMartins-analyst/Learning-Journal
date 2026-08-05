##  Day 1



- I learned how to use the select and where functions, along with operators like BETWEEN/NOT BETWEEN, AND/OR, IN/NOT IN and =,!=,<,<=,>,>=

- Practiced and completed a few exercises using this knowledge.



## Day 2



- = means EXACT match

- LIKE means PATTERN match

- % means "anything can go here"



## Day 3



I learned:



- WHERE filters data based on conditions.

- ORDER BY sorts the returned results.

- LIMIT restricts the number of rows returned.

- Typical query flow:

&#x20; SELECT → FROM → WHERE → ORDER BY → LIMIT

- Before writing SQL, define the business question you are trying to answer.

- The same SQL concept can be explained differently depending on the audience (business vs. technical).



## Day 4



- Reviewed SQLBolt Lesson 4 after realizing my mistake wasn't SQL syntax but requirement interpretation.



### Key takeaways

- Read requirements carefully before writing the query.

- "First" usually refers to the rows after applying `ORDER BY`, not the earliest records.

- Always ask: "First according to what?"



\### Reflection

A wrong answer doesn't always mean I misunderstood SQL. Sometimes I simply interpreted the business requirement differently. Finding the exact misunderstanding is part of becoming a better analyst.

## Day 5

Completed SQLBolt Lessons 5 and 6.

### Key takeaways
- `IN` checks whether a value belongs to a list of possible values.
- `OFFSET` specifies how many sorted rows SQL should skip.
- `JOIN` combines information from related tables.
- The `ON` clause defines which rows from each table should match.
- Without the correct join condition, SQL can produce many repeated combinations of rows.

### Reflection
Lesson 6 was straightforward once I understood that `ON` is what defines the relationship between the two tables. Forgetting it caused repeated movie names, but diagnosing the mistake helped clarify how joins work.

## Day 6 — Weekly Review

Reviewed filtering, sorting, pagination, and joins through a boss battle.

### Key takeaways
- `LIMIT` and `OFFSET` work together to select a section of an ordered result.
  - `OFFSET` decides where the section begins.
  - `LIMIT` decides how many rows are returned.
- The base table should be chosen by the result's grain: what one returned row represents.
- `JOIN` combines related data from different tables.
- `ON` matches rows by comparing related key values.
- `JOIN` normally means the same as `INNER JOIN`.
- Use single quotes for text values, such as `'Portugal'`.
- Qualifying column names with their table names makes joined queries clearer.

### Reflection
The review exposed a real misunderstanding about `LIMIT` and `OFFSET`. I also learned to distinguish between a logical mistake and English wording that does not accurately express my intended reasoning.

## Day 7

- Learned that `LEFT OUTER JOIN` and `RIGHT OUTER JOIN` keep all rows from one selected table, while `FULL OUTER JOIN` keeps all matching and unmatched rows from both tables.
- When an outer join preserves a row without a match, the missing side’s columns contain `NULL`.
- Practiced choosing the simplest query based on the requirement instead of forcing the newest SQL concept into every solution.