**Title:** Verify keyboard navigation functionality for title column links

**Preconditions:**
  1. At least one dashboard exists in the Dashboards table.

**Test Steps:**
  1. Login to the workspace as an authenticated user.
  2. Navigate to the Dashboard List page.
  3. Use Tab key to navigate to the first dashboard title link.
  4. Verify the link receives proper focus indicator.
  5. Press Enter to activate the link.
  6. Verify navigation to the dashboard detail page.
  7. Use Shift+Tab to navigate backwards through title links.
  8. Test keyboard navigation with screen reader enabled.

**Expected Result:**
* All dashboard title links are accessible via Tab navigation
* Links display clear focus indicators when selected
* Pressing Enter navigates to the correct dashboard detail page
* Tab order is logical and consistent
* Keyboard navigation works properly with assistive technologies
* Users can navigate backwards through links using Shift+Tab