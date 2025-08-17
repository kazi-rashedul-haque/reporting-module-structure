**Title:** Verify security validation and error handling.

**Test Steps:**
1. Login to the application as an authenticated user.
2. Navigate to the Reports page and open any report details.
3. Click on Actions dropdown and select "Add to Dashboard" button.
4. In the search field, attempt to enter HTML tags like `<script>alert('test')</script>`.
5. Verify HTML tags are properly sanitized and not executed.

**Expected Result:**
All user inputs should be properly sanitized and validated, HTML tags and script injections should be prevented