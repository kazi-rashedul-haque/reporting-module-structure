**Title:** Verify security validation against HTML and script injection in description.

**Test Steps:**
1. Login to the application as an authenticated user.
2. Navigate to the Reports page.
3. Click the Create Report button to open the modal.
4. Click on the Description field.
5. Enter HTML script tags `<script>alert('XSS')</script>`.
6. Verify system behavior for sanitization, rejection, or escaping.
7. Enter HTML formatting tags `<div>Test description</div>`.
8. Test image tag with onerror `<img src=x onerror=alert('XSS')>`.
9. Test link injection `<a href="javascript:alert('XSS')">Test</a>`.
10. Attempt to proceed with the Next button.
11. Verify no script execution occurs.

**Expected Result:**
The system should properly sanitize or escape HTML tags and scripts, reject input containing malicious HTML or scripts with appropriate error messages, strip HTML tags while keeping only text content, prevent any script execution from occurring, and implement security measures that effectively prevent XSS attacks through the description field.