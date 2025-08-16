# Verify Add Dataset functionality for multiple datasets

## Pre-conditions:
* At least one report exists in the report list
* The sidebar is currently expanded
* Table radio button is selected

## Test Steps:
1. Login to the workspace as an authenticated user.
2. Navigate to the Reporting page.
3. Select any existing report from the report table to open report details page.
4. Select Table from the Report Type options.
5. Configure Data Category, Time Frame, and Data Grouping in the first dataset.
6. Locate the "Add Dataset" button with icon in the Dataset section.
7. Click on the "Add Dataset" button.
8. Verify a new dataset configuration section appears with drag-to-reorder handle.
9. Configure the new dataset with different Data Grouping and Dataset parameters.
10. Verify both datasets show in the configuration with reorder handles and individual comboboxes.

## Expected Result:
* Add Dataset button should be visible and clickable with appropriate icon
* New dataset configuration section should appear with drag-to-reorder functionality
* Multiple datasets should be configurable independently with separate comboboxes
* Each dataset should have its own Data Grouping and Dataset selection
* Both datasets should be reflected in the table data display as separate rows
* Table supports unlimited datasets as per use case requirements