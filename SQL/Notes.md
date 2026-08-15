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

## Day 8

- Learned that `NULL` represents missing or unknown information rather than an ordinary value.
- Used `IS NULL` and `IS NOT NULL` because ordinary comparisons such as `= NULL` do not work.
- Practiced using `NULL` to identify matched and unmatched rows after an outer join.
- Learned that joined queries can qualify columns with full table names or shorter table aliases for clarity.

## Day 9

- Learned how SQL expressions can perform calculations on stored values without changing the underlying table.
- Used `AS` to give calculated result columns meaningful names.
- Practiced converting values using arithmetic expressions, such as converting a 0–10 rating into a percentage.
- Learned that `%` is the modulo operator and returns the remainder after division.
- `WHERE year % 2 = 0` keeps years whose division by 2 has a remainder of 0.
- Reinforced the principle of choosing the simplest query that answers the business requirement instead of forcing newly learned syntax into every solution.

## Day 10 — Week 2 Boss Battle

- Reviewed `INNER JOIN`, `LEFT OUTER JOIN`, `NULL`, expressions, aliases, sorting, and modulo.
- Reinforced that `NULL` means a specific field has a missing or unknown value; it is not limited to failed joins.
- Practiced using `LEFT OUTER JOIN` plus `IS NULL` to find records with no match in another table.
- Reinforced choosing the correct column for `IS NULL` based on the business question rather than simply testing any nullable field.
- Practiced calculated columns using expressions and `AS` without changing the stored table data.
- Reinforced using single quotes for SQL strings, such as `'Portugal'`.
- Practiced avoiding unnecessary joins when the required information already exists in one table.

## Day 11 — Aggregate Queries and GROUP BY

- Learned the aggregate functions `MAX`, `MIN`, `AVG`, `SUM`, and `COUNT`.
- An aggregate without `GROUP BY` summarizes the qualifying dataset into one overall result.
- `GROUP BY` divides rows into groups and calculates the aggregate separately for each group.
- Practiced calculating average employee tenure by role and total employee-years by building.
- Reinforced the difference between result grain and the measure being calculated.
  - Example: one row = one department is the grain.
  - Highest salary in that department is the measure.
- Reinforced that the aggregate function must match the business question: `SUM` and `COUNT` may both return valid numbers but represent different things.