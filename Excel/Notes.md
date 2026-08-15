## Day 1



- I learned to format tables, pivot tables and functions. I also learned XLOOKUP.

- I learned about the difference about aggregate, single output and spilled array formula.

- I built and formatted a functional table and pivot table with this knowledge.



## Day 2



What I remembered easily:

- Absolute references

- SUM

- Basic table layout

- XLOOKUP and how to retrieve information from outside tables

-. the use of F2 to edit a cell and F4 to make a cell's value absolute when using a function with an array of cells



What I had to think about:

- Percentage formula

- Column organization



## Day 3

What I learned:

- COUNT counts numeric cells only.

- COUNTA counts all non-empty cells.

- ROWS counts the number of rows, regardless of contents.

- Choose functions based on the business question, not on which one is "more powerful."

- Dynamic arrays spill automatically; use # to reference the entire spill range.

- SORT(UNIQUE(...)) is generally more efficient than UNIQUE(SORT(...)) because duplicates are removed before sorting.

- Think in terms of business problems first, formulas second.



## Day 4

Focused on understanding the logic behind array formulas instead of learning new functions.



### Key takeaways

- `IF` does not perform the logical test—it only decides what to return based on TRUE/FALSE.

- `+` works as OR, `\*` works as AND.

- Parentheses change the meaning of logical expressions (same principle as PEMDAS).

- Before choosing a formula, think about the business logic:

&#x20; - If conditions cannot overlap (e.g. 2024 OR 2025), separate `COUNTIFS` + addition is fine.

&#x20; - If conditions can overlap (e.g. 2024 OR Product = "Razer"), use logical array formulas to avoid double-counting.



### Reflection

Today's biggest improvement wasn't learning a new function—it was learning to translate business questions into logical expressions before writing formulas.

## Day 5

- - Repeated Day 3's homework as a retrieval exercise. I made a few logical mistakes, but identified and corrected them independently because I understood what each formula was instructing Excel to do.

## Day 6 — Weekly Review

Reviewed logical array formulas through retrieval and mixed business questions.

### Key takeaways
- Logical tests return TRUE/FALSE values.
- `+` represents OR and `*` represents AND.
- Parentheses determine which conditions belong together.
- `IF` converts any non-zero logical result into the chosen output.
- When OR conditions can overlap, separate counts may double-count the same row.
- Text criteria such as `"Portugal"` and `"Razer"` require quotation marks.

### Reflection
I retained the main concepts well. My biggest challenge was expressing the logic precisely in English, rather than understanding how the formulas worked.

## Day 7

- Reviewed Week 1 concepts to confirm that nested logical expressions, joins, and pagination had been consolidated.
- Learned that number formatting changes only how a value is displayed, while `ROUND` returns a new rounded value that later calculations can use.
- Understood why displayed values may appear not to equal a displayed total: Excel still calculates with the full stored precision.

## Day 8

- Learned how Excel stores dates as whole numbers and times as fractions of a day.
- Practiced calculating date durations, including using `+1` when both the start and end dates must be counted.
- Used `EDATE` to move a date by a number of months and `EOMONTH` to return the final day of a month.
- Calculated working hours by subtracting times and multiplying by 24, and used `MOD(...,1)` to handle shifts that cross midnight.


## Day 9

- Reviewed Day 8 material and reinforced the meaning of `NULL` before starting new content.
- Practiced `IF`, `AND`, `OR`, `ISNUMBER`, `ISTEXT`, comparison operators, and `IFNA`.
- Reinforced that logical tests return TRUE/FALSE, while `IF` determines what value should be returned for each result.
- Learned that `ISNUMBER` and `ISTEXT` only prove what a value is when they return TRUE; a FALSE result does not automatically identify the value's type.
- Learned that `IFNA` replaces only `#N/A` errors and otherwise returns the original result.
- Corrected a running-balance reference mistake: cumulative calculations must use the previous balance rather than repeatedly referencing the starting value.

## Day 10 — Week 2 Boss Battle

- Reviewed date and time logic, including inclusive date counting, `EDATE`, `EOMONTH`, and how Excel stores time as fractions of a day.
- Reinforced `IF`, `IFNA`, `ISNUMBER`, `ISTEXT`, and mixed AND/OR logic using `*`, `+`, and parentheses.
- Confirmed that `IFNA` should preserve the original result unless the formula returns `#N/A`.
- Reinforced the difference between a technical result and a business rule: `#N/A` means a lookup failed, while what to do with that result depends on the business requirement.
- Revisited result grain: one row should represent the entity the business question is asking about.

## Day 11 — Lookup, Filter and Selection Functions

- Reinforced `XLOOKUP` for flexible lookups that return a corresponding value.
- Learned that `LOOKUP` can be useful for simpler lookups when the lookup values are sorted in ascending order, such as tax brackets, commissions, or shipping-weight tables.
- Learned that `XMATCH` returns the relative position of a value within an array rather than returning a corresponding value.
- Learned to use `FILTER` to return all records that satisfy one or more logical conditions.
- Reviewed using `*` as AND logic inside `FILTER`.
- Learned that `SWITCH` can choose between different results or arrays based on a selected value.
- Practiced combining functions, such as using `SWITCH` to select a pricing table and `LOOKUP` to retrieve a value from it.
- Reinforced choosing functions based on the business requirement rather than using the most powerful function automatically.