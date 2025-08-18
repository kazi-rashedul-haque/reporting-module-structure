**Title:** Verify back button allows navigation when no unsaved changes exist.

**Test Steps:**
1. Login to the workspace as an authenticated user.
2. Navigate to the Reports page.
3. Open an existing report to view report details.
4. Do not make any changes to the report (keep all fields unchanged).
5. Click the Back button in the header.
6. Verify no warning modal appears.
7. Verify the user is immediately navigated back to the Reports page.
8. Verify the report details page is no longer visible.

**Expected Result:**
• Back button functions immediately without any blocking
• No warning modal is displayed
• User is navigated directly to the Reports page
• Navigation is smooth and uninterrupted
• No unsaved changes warning appears
• Page transition occurs without delay or confirmation