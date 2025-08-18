🧪 Edge Test Cases

---
* **Title**: Save as New with No Reports
* **Description**: Verify Save as New behavior when dashboard has no reports
* **Pre-Condition**: Dashboard is empty (no reports added)
* **Test Steps**:
  * Open Unsaved Changes dropdown on empty dashboard
  * Use "Save as New" functionality
  * Create new dashboard with valid name
* **Expected Result**:
  * New dashboard is created successfully
  * New dashboard is empty (no reports)
  * Dashboard structure and filters are preserved
  * User can add reports to new dashboard normally
---
* **Title**: Save as New with Maximum Reports
* **Description**: Verify Save as New with dashboard containing maximum number of reports
* **Pre-Condition**: Dashboard has maximum allowed number of reports
* **Test Steps**:
  * Create dashboard with maximum reports
  * Use "Save as New" functionality
* **Expected Result**:
  * All reports are preserved in new dashboard
  * Performance remains acceptable
  * New dashboard functions normally with all reports
  * No data loss occurs
---
* **Title**: Rapid Save as New Attempts
* **Description**: Verify behavior with rapid clicking of Save Changes button
* **Pre-Condition**: Save as New modal is open with valid data
* **Test Steps**:
  * Enter valid dashboard data
  * Rapidly click "Save Changes" multiple times
* **Expected Result**:
  * Only one save operation is executed
  * No duplicate dashboards are created
  * Proper loading state management
  * User feedback during processing
---
* **Title**: Save as New with Complex Filters
* **Description**: Verify Save as New preserves complex filter combinations
* **Pre-Condition**: Dashboard has multiple complex filters applied
* **Test Steps**:
  * Apply complex filter combinations (multiple campaigns, communities, time periods)
  * Use "Save as New" functionality
* **Expected Result**:
  * All filter combinations are preserved accurately
  * Filter settings work correctly in new dashboard
  * No filter conflicts or data loss
  * Dashboard displays filtered data correctly
---
* **Title**: Browser Navigation During Save as New
* **Description**: Verify behavior when user navigates away during Save as New process
* **Pre-Condition**: Save as New modal is open with unsaved data
* **Test Steps**:
  * Enter dashboard data
  * Press browser back button or navigate away
* **Expected Result**:
  * Appropriate warning about unsaved changes
  * Option to save or discard changes
  * Graceful handling of navigation
  * No partial dashboard creation
  * Original dashboard state preserved
---