**Title:** Verify print chart functionality

**Pre-conditions:**
* At least one user report exists in the report list with configured chart data

**Test Steps:**
1. Login to the workspace as an authenticated user.
2. Navigate to the Reporting page.
3. Select any existing report from the Reports table to open the report details page.
4. Ensure the chart is configured and displaying data in the main area.
5. Right-click on the chart to open the context menu.
6. Select "Print Chart" from the context menu.
7. Verify that the system print dialog opens. [Not supported in Playwright – use page.on('dialog') or mock print dialog]
8. Test the print preview functionality. [Not supported in Playwright – use CSS media queries validation]
9. Verify that the chart appears in print preview format. [For automation: verify print CSS is applied]

**Expected Result:**
* "Print Chart" option should be available in the chart context menu.
* Selecting this option should trigger the system print dialog. [For automation: verify print event is fired]
* The print preview should display the current chart view with proper formatting. [For automation: verify print-specific CSS is applied]
* The chart should be properly scaled and positioned for printing.
* Print settings should be accessible through the browser's print dialog. [For automation: verify print media query styles]