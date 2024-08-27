---
hide:
  - tags
  - footer
tags:
  - Catalogs
  - GREP
---

# **GREP**


{==

## **Paragraph Styles**

==}

- When certain text needs a specific character style


---


{==

## **Find/Change dialog box**

==}

- When certain text needs to be added, removed, or replaced
- Change to: $1 (Found Text 1)


---


{==

## **Expressions**

==}

| GREP | Description | Notes |
| :----- | :---------- | :---- |
| + | One or More Times |  |
| +? | One or More Times (Shortest Match) |  |
| .+ | One or More Times (Any Character) |  |
| () | Sub-Expressions | Place one or more expressions inside parentheses |
| ? | Shortest Match |  |


---


**Find multiple words/phrases**

    cooking|cooks|cook

- If “cook” is listed first, it would skip over “cooks” and “cooking”


---


{==

## **Formatting Fractions**

==}

\d+/\d+

Any White Space - finds space at end of previous line?

\s\d+/\d+

Posix [[=a=]] - Winner?

[[= =]]\d+/\d+

Posix [[:space:]] - finds space at end of previous line?

[[:space:]]\d+/\d+


---
