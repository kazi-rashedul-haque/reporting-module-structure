✅ Positive Test Cases

---
* **Title**: Save as New Button Visibility
* **Description**: Verify Save as New button is visible and accessible in Unsaved Changes dropdown
* **Pre-Condition**: Dashboard has unsaved changes and Unsaved Changes dropdown is open
* **Test Steps**:
  * Make changes to dashboard (add/remove reports, modify filters)
  * Open Unsaved Changes dropdown
  * Locate "Save as New" button in dropdown
* **Expected Result**:
  * "Save as New" button is visible in Unsaved Changes dropdown
  * Button is enabled and clickable
  * Button text displays "Save as New"
---
* **Title**: Save as New Modal Opens
* **Description**: Verify clicking Save as New button opens Create Dashboard modal
* **Pre-Condition**: Dashboard has unsaved changes and Unsaved Changes dropdown is open
* **Test Steps**:
  * Click on "Save as New" button in dropdown
* **Expected Result**:
  * Create Dashboard modal opens
  * Modal has title "Create Dashboard"
  * Unsaved Changes dropdown closes
  * Form fields are empty and ready for input
---
* **Title**: Modal Structure Validation
* **Description**: Verify Save as New modal contains all required elements
* **Pre-Condition**: Save as New modal is open from Unsaved Changes dropdown
* **Test Steps**:
  * Open Save as New modal
  * Verify all modal elements are present
* **Expected Result**:
  * Modal title: "Create Dashboard"
  * Close button (X) in top-right corner
  * Dashboard Name field with label "Dashboard Name*" and placeholder "Enter name"
  * Description field with placeholder "Write description"
  * Cancel button
  * Save Changes button
---
* **Title**: Dashboard Name Field Validation
* **Description**: Verify dashboard name field properties and requirements in Save as New flow
* **Pre-Condition**: Save as New modal is open
* **Test Steps**:
  * Examine Dashboard Name field
  * Test field behavior and validation rules
* **Expected Result**:
  * Field label: "Dashboard Name*" (asterisk indicates required)
  * Placeholder text: "Enter name"
  * Field is empty initially
  * Field is required (mandatory for form submission)
  * Maximum length: 120 characters
  * HTML tags are not allowed in input
---
* **Title**: Description Field Validation
* **Description**: Verify description field properties and requirements in Save as New flow
* **Pre-Condition**: Save as New modal is open
* **Test Steps**:
  * Examine Description field
  * Test field behavior and validation rules
* **Expected Result**:
  * Placeholder text: "Write description"
  * Field is empty initially
  * Field is optional (not required for submission)
  * Maximum length: 240 characters
  * HTML tags are not allowed in input
---
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
---
* **Title**: Current State Preservation
* **Description**: Verify all current dashboard state is preserved in new dashboard
* **Pre-Condition**: Dashboard has specific reports, filters, and configurations applied
* **Test Steps**:
  * Add specific reports to dashboard
  * Apply filters (time period, campaign, community)
  * Configure report settings
  * Use "Save as New" functionality with valid name
* **Expected Result**:
  * New dashboard contains all currently visible reports
  * All applied filters are preserved in new dashboard
  * Report configurations and time frames are maintained
  * Dashboard layout and report positions are preserved
---
* **Title**: Cancel Button Functionality
* **Description**: Verify Cancel button returns to original dashboard without saving
* **Pre-Condition**: Save as New modal is open with some input
* **Test Steps**:
  * Enter some text in Dashboard Name and/or Description
  * Click "Cancel" button
* **Expected Result**:
  * Modal closes without saving
  * No new dashboard is created
  * User remains on current dashboard with unsaved changes
  * Input data is discarded
  * Original dashboard state is unchanged
---
* **Title**: Close Button Functionality
* **Description**: Verify X (close) button returns to original dashboard without saving
* **Pre-Condition**: Save as New modal is open with some input
* **Test Steps**:
  * Enter some text in Dashboard Name and/or Description
  * Click X (close) button
* **Expected Result**:
  * Modal closes without saving
  * No new dashboard is created
  * User remains on current dashboard with unsaved changes
  * Input data is discarded
---