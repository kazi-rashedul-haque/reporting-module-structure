**Title:** Verify handling of duplicate dashboard names during creation

**Preconditions:**
At least one dashboard already exists in the system.

**Test Steps:**
1. Login to the workspace as an authenticated user.
2. Navigate to the Dashboard List page.
3. Go to the Dashboard List page.
4. Note an existing dashboard name (e.g., “Build Test 5 June”).
5. Click Create Dashboard button.
6. Enter the same name (“Build Test 5 June”) in the Name field.
7. Enter description: “Test duplicate validation”.
8. Click Save Changes → observe system response.
9. Try again with same name but different case: “BUILD TEST 5 JUNE”.
10. Try again with same name but with leading/trailing spaces: “ Build Test 5 June ”.
11. Change the name to a unique value (e.g., “Build Test 5 June - Copy”) and submit.

**Expected Result:**

* Duplicate name is detected, dashboard is not created.
* Error message shown: “A dashboard with this name already exists. Please choose a different name.”
* Case-insensitive match triggers the same error.
* Leading/trailing spaces are trimmed before validation.
* Error appears clearly near the Name field.
* Save Changes button does not proceed while error exists.
* User can correct the name to something unique.
* Once unique, submission succeeds and dashboard is created.
* Error message disappears immediately when unique input is entered.
* System may suggest alternatives (e.g., appending “(Copy)”).