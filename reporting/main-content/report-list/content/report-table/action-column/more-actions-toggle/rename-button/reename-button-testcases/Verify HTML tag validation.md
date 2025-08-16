**Title:** Verify HTML tag validation in report name and description fields

**Preconditions:**
  1. At least one user-created report exists in the Reports table.

**Test Steps:**
  1. Login to the workspace as an authenticated user.
  2. Navigate to the Reports page.
  3. Click on the "More Actions" button (three dots) for any report.
  4. Click on "Rename" from the dropdown menu.
  5. Enter HTML tags in the "Report Name" field (e.g., "<script>alert('test')</script>", "<div>test</div>").
  6. Enter HTML tags in the "Description" field with various HTML elements.
  7. Test with HTML entities like &lt;, &gt;, &amp;.
  8. Attempt to save the changes.

**Expected Result:**
  The system should reject or sanitize HTML tags in both fields, appropriate validation messages should appear when HTML tags are detected, HTML entities should be handled appropriately (either converted or rejected), the system should prevent potential XSS vulnerabilities, and valid special characters (non-HTML) should still be allowed.