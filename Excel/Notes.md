\## Day 1



I learned to format tables, pivot tables and functions. I also learned XLOOKUP.

I learned about the difference about aggregate, single output and spilled array formula.

I built and formatted a functional table and pivot table with this knowledge.



\## Day 2



What I remembered easily:

\- Absolute references

\- SUM

\- Basic table layout

\- XLOOKUP and how to retrieve information from outside tables

\-. the use of F2 to edit a cell and F4 to make a cell's value absolute when using a function with an array of cells



What I had to think about:

\- Percentage formula

\- Column organization



\## Day 3

What I learned:

\- COUNT counts numeric cells only.

\- COUNTA counts all non-empty cells.

\- ROWS counts the number of rows, regardless of contents.

\- Choose functions based on the business question, not on which one is "more powerful."

\- Dynamic arrays spill automatically; use # to reference the entire spill range.

\- SORT(UNIQUE(...)) is generally more efficient than UNIQUE(SORT(...)) because duplicates are removed before sorting.

\- Think in terms of business problems first, formulas second.



\## Day 4

Focused on understanding the logic behind array formulas instead of learning new functions.



\### Key takeaways

\- `IF` does not perform the logical test—it only decides what to return based on TRUE/FALSE.

\- `+` works as OR, `\*` works as AND.

\- Parentheses change the meaning of logical expressions (same principle as PEMDAS).

\- Before choosing a formula, think about the business logic:

&#x20; - If conditions cannot overlap (e.g. 2024 OR 2025), separate `COUNTIFS` + addition is fine.

&#x20; - If conditions can overlap (e.g. 2024 OR Product = "Razer"), use logical array formulas to avoid double-counting.



\### Reflection

Today's biggest improvement wasn't learning a new function—it was learning to translate business questions into logical expressions before writing formulas.

## Day 5

- - Repeated Day 3's homework as a retrieval exercise. I made a few logical mistakes, but identified and corrected them independently because I understood what each formula was instructing Excel to do.
