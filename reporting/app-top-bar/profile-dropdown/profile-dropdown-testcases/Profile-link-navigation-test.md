**Title:** Verify profile link navigation to member profile page

**Pre-conditions:**
* User is logged in as an authenticated user

**Test Steps:**
1. Login to the workspace as an authenticated user.
2. Navigate to Dashboard page .
3. Click on the profile avatar button to open the dropdown.
4. Locate the profile link at the top of the dropdown menu.
5. Verify the profile link displays:
   - User avatar image
   - Full name "Super user"
   - Username "@superuser"
6. Click on the profile link.
7. Verify navigation occurs to the member profile page.
8. Check that the URL contains "/c/member-profile/1".

**Expected Result:**
* Profile link displays complete user information with avatar, name, and username
* Link is clickable
* Clicking the profile link navigates to "/c/member-profile/1"
* Full name and username are displayed correctly on the member profile page