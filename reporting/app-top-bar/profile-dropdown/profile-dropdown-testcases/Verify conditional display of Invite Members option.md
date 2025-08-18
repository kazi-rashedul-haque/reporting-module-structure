**Title:** Verify conditional display of "Invite Members" option

**Preconditions:**
1. User is logged in as an admin
2. Admin can enable/disable the Invite Members feature in workspace settings

**Test Steps:**
1. Go to workspace settings >> Security tab >> Auto-Approve List Section.
2. Turn ON the Invite Members feature.
3. Go to the Dashboard Page → open profile dropdown.
4. Confirm Invite Members option is shown.
5. Go back to settings and turn OFF the Invite Members feature.
6. Return to Dashboard → open profile dropdown.
7. Confirm Invite Members option is Not visible.

**Expected Result:**
* When OFF → Invite Members is hidden, dropdown layout is normal.
* When ON → Invite Members is shown with correct icon and position.