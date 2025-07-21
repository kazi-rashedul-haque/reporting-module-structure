### Positive Use Cases:
1. User clicks `Cancel` to dismiss changes:
   * Any unsaved changes are discarded. 

2. User clicks `Cancel` to close the form/modal:
   * The `Cancel` button should close the modal and return the user to Report Creation page without applying any changes.

### Negative Use Cases:
1. User clicks `Cancel` after changes were made, but changes persist:
   * Clicking the `Cancel` button should discard any unsaved changes.

2. User clicks `Cancel` with no changes:
   * The system should close the form without any errors or warnings if no changes have been made.

### Edge Use Cases:
1. User clicks `Cancel` after a long wait:
   * If the system is slow (e.g., network delay), the user may click `Cancel` mid-process. The form should handle this gracefully and cancel any ongoing requests or processes.

### Accessibility Use Cases:
1. `Cancel` button is focusable and accessible via keyboard navigation:
   * Users should be able to navigate to the `Cancel` button using the `Tab` key and activate it with the `Enter` key.

2. `Cancel` button announced by screen readers:
   * The screen reader should announce the button with accessible text like `Cancel` when focused.

3. `Cancel` button is distinguishable and provides visual feedback:
   * The button should have sufficient contrast and provide feedback on hover or focus (e.g., change in color or border).