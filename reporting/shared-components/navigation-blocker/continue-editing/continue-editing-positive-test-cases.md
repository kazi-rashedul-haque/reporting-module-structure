✅ Positive Test Cases

---
* **Title**: Continue Editing Button Visibility
* **Description**: Verify Continue Editing button is visible and accessible in warning modal
* **Pre-Condition**: User attempts navigation with unsaved changes, triggering navigation warning modal
* **Test Steps**:
  * Make changes to dashboard (add/remove reports, modify filters)
  * Attempt to navigate away (click another dashboard, browser navigation, etc.)
  * Observe warning modal that appears
  * Locate "Continue Editing" button in modal
* **Expected Result**:
  * Warning modal appears with navigation blocked
  * "Continue Editing" button is visible in modal
  * Button is enabled and clickable
  * Button text displays "Continue Editing"
---
* **Title**: Continue Editing Button Functionality
* **Description**: Verify clicking Continue Editing button closes modal and remains on current dashboard
* **Pre-Condition**: Navigation warning modal is open with Continue Editing button visible
* **Test Steps**:
  * Click on "Continue Editing" button
* **Expected Result**:
  * Warning modal closes immediately
  * User remains on current dashboard view
  * Navigation is cancelled/blocked
  * Unsaved changes are preserved
  * Dashboard remains in its current state
---
* **Title**: Dashboard State Preservation
* **Description**: Verify dashboard state is completely preserved after clicking Continue Editing
* **Pre-Condition**: Dashboard has specific unsaved changes applied
* **Test Steps**:
  * Add specific reports to dashboard
  * Apply filters (time period, campaign, community)
  * Modify report configurations
  * Attempt navigation to trigger warning modal
  * Click "Continue Editing"
  * Verify all changes are still present
* **Expected Result**:
  * All added reports remain visible and functional
  * All applied filters are still active
  * Report configurations are preserved
  * Dashboard layout remains unchanged
  * All unsaved changes indicator remains active
---
* **Title**: Focus Return After Continue Editing
* **Description**: Verify proper focus management after clicking Continue Editing
* **Pre-Condition**: Navigation warning modal is open
* **Test Steps**:
  * Click "Continue Editing" button
  * Observe where focus is placed after modal closes
* **Expected Result**:
  * Focus returns to the last active element before navigation attempt
  * Focus is not lost or placed inappropriately
  * User can continue interaction seamlessly
  * Keyboard navigation continues from expected location
---
* **Title**: Multiple Continue Editing Actions
* **Description**: Verify Continue Editing works consistently across multiple navigation attempts
* **Pre-Condition**: Dashboard has unsaved changes
* **Test Steps**:
  * Attempt navigation and click "Continue Editing"
  * Make additional changes to dashboard
  * Attempt navigation again and click "Continue Editing"
  * Repeat process multiple times
* **Expected Result**:
  * Continue Editing works consistently each time
  * Modal behavior is identical across attempts
  * All changes accumulate properly
  * No degradation in functionality
  * Warning modal continues to trigger appropriately
---
* **Title**: Continue Editing from Different Navigation Triggers
* **Description**: Verify Continue Editing works from various navigation trigger sources
* **Pre-Condition**: Dashboard has unsaved changes
* **Test Steps**:
  * Test Continue Editing from dashboard selection dropdown navigation
  * Test Continue Editing from browser back/forward navigation
  * Test Continue Editing from direct URL navigation
  * Test Continue Editing from sidebar navigation
* **Expected Result**:
  * Continue Editing works consistently from all navigation sources
  * Modal appearance and behavior is identical
  * Navigation blocking is effective for all trigger types
  * Dashboard state preservation works universally
---
* **Title**: Continue Editing with Different Change Types
* **Description**: Verify Continue Editing preserves different types of unsaved changes
* **Pre-Condition**: Various types of changes made to dashboard
* **Test Steps**:
  * Test with only report additions
  * Test with only filter modifications
  * Test with only report configuration changes
  * Test with mixed change types
  * Use Continue Editing for each scenario
* **Expected Result**:
  * Continue Editing preserves all types of changes accurately
  * No data loss occurs regardless of change type
  * Dashboard functionality remains intact
  * All change indicators work correctly
---