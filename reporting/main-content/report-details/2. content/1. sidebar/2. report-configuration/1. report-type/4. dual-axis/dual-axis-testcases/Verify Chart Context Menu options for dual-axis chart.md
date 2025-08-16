**Title:** Verify Chart Context Menu options for dual-axis chart

**Pre-conditions:**
* User is logged in to the workspace
* At least one report exists with dual-axis chart type configured and displaying data
* Chart is fully rendered with both bar and line components visible

**Test Steps:**
1. Navigate to the Reporting page.
2. Select an existing report to open the report details page.
3. Ensure the dual-axis chart is displaying data with both bar and line components.
4. Right-click on the chart area to open the context menu.
5. Verify the context menu displays all expected options:
   - View in full screen
   - Print chart
   - Download PNG image
   - Download JPEG image
   - Download PDF document
   - Download SVG vector image
6. Click "View in full screen" and verify the chart opens in full screen mode.
7. Exit full screen mode and return to normal view.
8. Click "Print chart" and verify print dialog opens. [Not supported in Playwright – use API validation or mock print dialog]
9. Click "Download PNG image" and verify PNG file is generated. [Not supported in Playwright – use API validation or mock download]
10. Click "Download JPEG image" and verify JPEG file is generated. [Not supported in Playwright – use API validation or mock download]
11. Click "Download PDF document" and verify PDF file is generated. [Not supported in Playwright – use API validation or mock download]
12. Click "Download SVG vector image" and verify SVG file is generated. [Not supported in Playwright – use API validation or mock download]
13. Verify all downloaded files contain the complete dual-axis chart with both bar and line components.

**Expected Result:**
* Right-click context menu appears with all specified options
* "View in full screen" functionality works correctly
* Full screen mode displays the complete dual-axis chart properly
* Print option triggers appropriate print dialog
* All download options generate files in their respective formats
* Downloaded files contain high-quality representations of the dual-axis chart
* Both bar and line chart components are preserved in all export formats
* Chart legend and axes are included in all exported versions
* File names are descriptive and include appropriate timestamps or identifiers