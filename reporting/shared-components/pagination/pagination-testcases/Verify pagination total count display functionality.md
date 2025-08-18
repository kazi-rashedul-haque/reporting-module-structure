**Title:** Verify pagination total count display functionality

**Preconditions:**
* At least 21 {ITEM_TYPE_PLURAL} exist in the system to ensure pagination displays multiple pages

**Test Steps:**
1. Login to the workspace as an authenticated user.
2. Navigate to the {PAGE_NAME} page.
3. Verify that the pagination count text is displayed at the bottom left of the table.
4. Verify the count text shows the correct format: "Displaying X - Y of Z {ITEM_TYPE_PLURAL_CAPITALIZED}".
5. Verify the current page range (X - Y) matches the number of {ITEM_TYPE_PLURAL} visible in the table.
6. Verify the total count (Z) represents the actual total number of {ITEM_TYPE_PLURAL} in the system.
7. Navigate to page 2 using the pagination controls.
8. Verify the count text updates to show the correct range for page 2.
9. Change the page size from default (20) to 10 using the page size dropdown.
10. Verify the count text updates to reflect the new page size: "Displaying 1 - 10 of Z {ITEM_TYPE_PLURAL_CAPITALIZED}".
11. Navigate to the last page.
12. Verify the count text shows the correct range for the final page (may be partial).
13. Search for a specific {ITEM_TYPE} to filter the results.
14. Verify the count text updates to show filtered results count.
15. Clear the search filter.
16. Verify the count text returns to show total unfiltered count.

**Expected Result:**
* Count text is always visible in the bottom left of the pagination area
* Format follows pattern: "Displaying [start] - [end] of [total] {ITEM_TYPE_PLURAL_CAPITALIZED}"
* Current page range (start - end) accurately reflects visible {ITEM_TYPE_PLURAL}:
  - Page 1 with 20 items: "Displaying 1 - 20 of 28 {ITEM_TYPE_PLURAL_CAPITALIZED}"
  - Page 2 with 20 items: "Displaying 21 - 28 of 28 {ITEM_TYPE_PLURAL_CAPITALIZED}" (if 28 total)
* Total count (Z) remains consistent across pages unless filtered
* Range updates correctly when page size changes:
  - 10 items per page: "Displaying 1 - 10 of 28 {ITEM_TYPE_PLURAL_CAPITALIZED}"
  - 30 items per page: "Displaying 1 - 28 of 28 {ITEM_TYPE_PLURAL_CAPITALIZED}" (if 28 total)
* Count text updates immediately when pagination controls are used
* Filtered search shows filtered count: "Displaying 1 - X of Y {ITEM_TYPE_PLURAL_CAPITALIZED}" where Y ≤ total
* Text formatting and spacing remain consistent across all states
* Numbers are accurate and never show impossible ranges (e.g., "21 - 20")