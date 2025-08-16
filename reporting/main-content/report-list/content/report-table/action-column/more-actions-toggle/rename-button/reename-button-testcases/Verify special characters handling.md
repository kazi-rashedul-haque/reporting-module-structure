**Title:** Verify handling of special characters in report rename

**Preconditions:**
  1. At least one user-created report exists in the Reports table.

**Test Steps:**
  1. Login to the workspace as an authenticated user.
  2. Navigate to the Reports page.
  3. Click on the "More Actions" button (three dots) for any report.
  4. Click on "Rename" from the dropdown menu.
  5. Test various special characters in both name and description fields:
     - Quotes: single ('), double (")
     - Numbers and symbols: @, #, $, %, &, -, _
     - Parentheses and brackets: (), [], {}
  6. Attempt to save with valid special character combinations
  7. Test edge cases like names with only spaces or special characters.


**Expected Result:**
* Valid special characters accepted and saved correctly
• Quotes and apostrophes accepted and saved correctly
• Names containing only spaces accepted and saved as valid
• Renamed report displays special characters correctly in the table