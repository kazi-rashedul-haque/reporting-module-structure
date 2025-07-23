✅ Positive Test Cases

---
* **Title**: Collapse Sidebar Button Visibility
* **Description**: Ensure the collapse button is visible and enabled when the dashboard is loaded.
* **Pre-Condition**: User is logged in and navigated to the Dashboard view.
* **Test Steps**:
  * Navigate to the Dashboard view.
  * Observe the header section near the “Legacy Dashboard” title.
* **Expected Result**:
  * The collapse/expand button is present.
  * The button is visible and enabled (not disabled or hidden).
---
* **Title**: Collapse Sidebar on Click
* **Description**: Clicking the collapse button should collapse the sidebar.
* **Pre-Condition**: Sidebar is expanded initially.
* **Test Steps**:
  * Navigate to the Dashboard view.
  * Ensure the sidebar is currently expanded.
  * Click the collapse button once.
* **Expected Result**:
  * Sidebar collapses.
  * The button icon updates to reflect the “expand” state.
  * The tooltip changes to "Expand sidebar" on hover.
---
* **Title**: Expand Sidebar on Click
* **Description**: Clicking the expand button should expand the sidebar.
* **Pre-Condition**: Sidebar is collapsed initially.
* **Test Steps**:
  * Navigate to the Dashboard view.
  * Collapse the sidebar by clicking the collapse button.
  * Click the button again to expand the sidebar.
* **Expected Result**:
  * Sidebar expands.
  * The button icon updates to reflect the “collapse” state.
  * The tooltip changes to "Collapse sidebar" on hover.
---
* **Title**: Tooltip Display on Hover
* **Description**: Verify that the appropriate tooltip is shown when hovering over the collapse/expand button.
* **Pre-Condition**: Dashboard is open; sidebar in either state.
* **Test Steps**:
  * Hover over the collapse/expand button.
* **Expected Result**:
  * If sidebar is expanded: Tooltip shows "Collapse sidebar".
  * If sidebar is collapsed: Tooltip shows "Expand sidebar".
---