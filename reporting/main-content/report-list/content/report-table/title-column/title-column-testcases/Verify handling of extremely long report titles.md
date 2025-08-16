**Title:** Verify handling of extremely long report titles

**Preconditions:**
  1. Reports with very long titles (120 characters) exist in the Reports table.

**Test Steps:**
  1. Login to the workspace as an authenticated user.
  2. Navigate to the Reports page.
  3. Locate reports with maximum length titles (120 characters).
  4. Verify that the title column displays these long titles correctly.

**Expected Result:**
* The title column should display the full report title without truncation.