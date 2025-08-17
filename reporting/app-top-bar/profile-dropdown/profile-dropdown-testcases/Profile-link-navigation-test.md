**Title:** Verify profile link navigation to member profile page

**Pre-conditions:**
* User is logged in as an authenticated user

**Test Steps:**
1. Login to the workspace as an authenticated user.
2. Navigate to Dashboard page in the application.
3. Click on the profile avatar button to open the dropdown.
4. Locate the profile link at the top of the dropdown menu.
5. Verify the profile link displays:
   - User avatar image
   - Full name "Super user"
   - Username "@superuser"
6. Click on the profile link.
7. Verify navigation occurs to the member profile page.
8. Check that the URL contains "/c/member-profile/1".
9. Verify the profile page loads correctly with user information.
10. Navigate back to test the link functionality again.

**Expected Result:**
* Profile link displays complete user information with avatar, name, and username
* Link is clickable and properly styled
* Clicking the profile link navigates to "/c/member-profile/1"
* Profile page loads successfully showing user details
* Navigation occurs in the same tab/window
* User information displayed in dropdown matches profile page data
* Avatar image loads correctly in both dropdown and profile page
* Link hover state provides appropriate visual feedback