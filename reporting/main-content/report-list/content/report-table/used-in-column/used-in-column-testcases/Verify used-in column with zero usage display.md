**Title:** Verify used-in column with zero usage display

**Preconditions:**
  1. At least one report exists that is not used in any dashboards.

**Test Steps:**
1. Login to the workspace as an authenticated user.
2. Navigate to the Reports page via Apps > Reporting NEW - Beta > Reports.
3. Locate reports that have zero dashboard usage in the "Used in" column.
4. Verify these reports show empty cells (no text or buttons).
5. Check that empty cells maintain proper table alignment.
6. Verify no click functionality exists for empty used-in cells.

**Expected Result:**
* Reports with zero dashboard usage display empty cells in "Used in" column
* Empty cells show no text, buttons, or interactive elements