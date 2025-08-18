**Title**: Save Changes Success Flow

* **Title**: Save Changes Success Flow
* **Description**: Verify successful dashboard creation preserving current state
* **Pre-Condition**: Save as New modal is open with dashboard having unsaved changes
* **Test Steps**:
  * Enter valid dashboard name (e.g., "My Dashboard Copy")
  * Optionally enter description
  * Click "Save Changes" button
* **Expected Result**:
  * New dashboard is created successfully with current state preserved
  * Modal closes
  * User is redirected to newly created dashboard view
  * All previously selected reports are added and displayed in report-area
  * Current filters and configurations are preserved in new dashboard
  * New dashboard appears in dashboard selection dropdown