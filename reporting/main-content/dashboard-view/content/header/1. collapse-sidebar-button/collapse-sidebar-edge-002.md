**Test Case ID**: TC_COLLAPSE_SIDEBAR_EDGE_002
**Title**: Conflict With External Sidebar Trigger
**Description**: Ensure collapse button works even if sidebar state changed by another method (e.g., shortcut key).
**Pre-Condition**: Sidebar was collapsed or expanded via another method.
**Test Steps**:
  * Change sidebar state using an external trigger.
  * Click the header collapse/expand button.
**Expected Result**:
  * Button remains functional.
  * Sidebar toggles state as expected.
  * No desynchronization in button icon or tooltip.