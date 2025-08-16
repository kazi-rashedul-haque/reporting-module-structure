**Title:** Verify Chart Legend display for dual-axis chart

**Pre-conditions:**
* User is logged in to the workspace
* At least one report exists with dual-axis chart type configured
* Chart is displaying data with both Y Axis Left (Bar) and Y Axis Right (Line) configured
* Additional datasets may be added to either axis

**Test Steps:**
1. Navigate to the Reporting page.
2. Select an existing report to open the report details page.
3. Ensure the dual-axis chart is displaying with both bar and line components.
4. Locate the chart legend in the top-right corner of the chart.
5. Verify the legend displays entries for Y Axis Left (Bar) data series.
6. Verify the legend displays entries for Y Axis Right (Line) data series.
7. Check that legend items use colors that match their corresponding chart elements.
8. Verify legend items for bar chart components show appropriate bar/rectangle indicators.
9. Verify legend items for line chart components show appropriate line indicators.
10. If additional datasets are configured, verify they appear in the legend with distinct colors.
11. Test clicking on legend items to toggle visibility of corresponding chart elements.
12. Verify legend text is readable and properly formatted.
13. Check that the legend positioning doesn't obscure chart data.
14. Test legend behavior when chart is resized or viewed in different screen sizes.

**Expected Result:**
* Chart legend appears in the top-right corner of the chart
* Legend displays all active data series for both Y Axis Left (Bar) and Y Axis Right (Line)
* Legend item colors match their corresponding chart elements exactly
* Bar chart legend items use appropriate bar/rectangle visual indicators
* Line chart legend items use appropriate line visual indicators
* Additional datasets (if any) appear in legend with distinct, accessible colors
* Clicking legend items toggles visibility of corresponding chart elements
* Legend text is readable with proper font size and contrast
* Legend positioning doesn't interfere with chart data visualization
* Legend adapts appropriately to different screen sizes and chart dimensions
* Legend maintains functionality and readability across all viewport sizes