**Title:** Verify chart context menu download options

**Pre-conditions:**
* At least one user report exists in the report list with configured chart data

**Test Steps:**
1. Login to the workspace as an authenticated user.
2. Navigate to the Reporting page.
3. Select any existing report from the Reports table to open the report details page.
4. Ensure the chart is configured and displaying data in the main area.
5. Right-click on the chart to open the context menu.
6. Verify that download options are available in the context menu.
7. Test each download format:
   - PNG
   - JPEG
   - PDF
   - SVG
8. Verify that each download option successfully exports the chart. [Not supported in Playwright – use API validation or mock download]

**Expected Result:**
* Right-clicking on the chart should open a context menu.
* Download options should be available with the following formats: PNG, JPEG, PDF, SVG.
* Each download option should trigger the download process. [For automation: verify download request is initiated]
* Downloaded files should contain the complete chart visualization with proper formatting. [For automation: verify download API response]