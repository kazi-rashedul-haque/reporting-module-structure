**Title:** Verify report name shows broken formatting with HTML, emoji, or script injection

**Test Steps:**
1. Login to the workspace as an authenticated user.
2. Navigate to the Reports page.
3. Create or modify a report name to include HTML tags (e.g., &lt;script&gt;, &lt;b&gt;, &lt;img&gt;).
4. Create or modify a report name to include emoji characters.
5. Create or modify a report name to include script injection attempts.
6. Open the report details page for each test case.
7. Examine how the report name displays in the header.
8. Verify that HTML tags are either escaped or stripped.
9. Check for any script execution or security vulnerabilities.
10. Document any broken formatting or display issues.

**Expected Result:**
* HTML tags should be escaped or stripped, not rendered as HTML.
* Script injection attempts should be neutralized and not execute.
* Emoji characters may show broken formatting or be displayed as text.
* No security vulnerabilities should be present.
* Any formatting issues should be contained and not affect the overall layout.