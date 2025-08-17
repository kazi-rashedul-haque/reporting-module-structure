**Title:** Verify workspace logo click functionality for home navigation

**Pre-conditions:**
* User is logged in as an authenticated user

**Test Steps:**
1. Login to the workspace as an authenticated user.
2. Navigate to Dashboard page in the application.
3. Navigate to any sub-page within the application (reports, settings, etc.).
4. Locate the workspace logo in the top navigation bar.
5. Verify the logo appears clickable (cursor changes to pointer on hover).
6. Click on the workspace logo.
7. Verify navigation occurs to the workspace home page.
8. Check that the URL changes to the home/main workspace URL.
9. Test logo click functionality from different pages in the application.
10. Verify logo click works consistently across different browsers.
11. Test keyboard accessibility by focusing on logo and pressing Enter.

**Expected Result:**
* Workspace logo shows pointer cursor on hover indicating it's clickable
* Clicking the logo navigates to the workspace home page
* Navigation occurs to the correct home URL (typically "/c")
* Logo click functionality works from any page within the application
* Navigation maintains user's authenticated session
* Page loads successfully after logo click
* Browser history is properly updated with navigation
* Logo click provides consistent behavior across all browsers
* Logo is keyboard accessible and can be activated with Enter key
* No JavaScript errors occur during logo click navigation
* Navigation occurs in the same tab/window