**Title:** Verify placeholder message when no data is selected

**Pre-conditions:**
* User has access to create new reports

**Test Steps:**
1. Login to the workspace as an authenticated user.
2. Navigate to the Reporting page.
3. Click the "Create Report" button.
4. Enter a report name in the modal (e.g., "Test Report").
5. Click "Next" button to proceed to the report creation page.
6. Observe the main chart area (right side of the screen) in its initial state.
7. Verify that the sidebar shows default report configuration options (Line chart selected, "Choose" buttons for Time Frame and Y Axis).
8. Verify the placeholder content in the main area.

**Expected Result:**
* A placeholder should be displayed in the main chart area when no data is fully configured.
* The placeholder should contain an image with alt text.
* The placeholder message should read exactly: "Choose your data to start building your report". .