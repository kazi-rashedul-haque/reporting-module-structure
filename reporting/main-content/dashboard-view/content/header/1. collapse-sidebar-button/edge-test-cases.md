🧪 Edge Test Cases

---
* **Title**: Sidebar Behavior on Different Screen Sizes
* **Description**: Validate correct collapse/expand behavior on various screen sizes (desktop, tablet, mobile).
* **Pre-Condition**: Application supports responsive layout.
* **Test Steps**:
  * Set viewport to desktop, tablet, and mobile widths.
  * Click the collapse/expand button.
* **Expected Result**:
  * Sidebar collapses/expands correctly on all screen sizes.
  * No layout shifts or broken UI elements.
---
* **Title**: Conflict With External Sidebar Trigger
* **Description**: Ensure collapse button works even if sidebar state changed by another method (e.g., shortcut key).
* **Pre-Condition**: Sidebar was collapsed or expanded via another method.
* **Test Steps**:
  * Change sidebar state using an external trigger.
  * Click the header collapse/expand button.
* **Expected Result**:
  * Button remains functional.
  * Sidebar toggles state as expected.
  * No desynchronization in button icon or tooltip.
---
* **Title**: Sidebar Animation Smoothness
* **Description**: Validate that collapse/expand transition has proper animation and isn’t broken or delayed.
* **Pre-Condition**: Default Dashboard view.
* **Test Steps**:
  * Click the collapse/expand button.
  * Observe the sidebar animation.
* **Expected Result**:
  * Animation should play smoothly.
  * No lag, jitter, or incomplete transition.
---