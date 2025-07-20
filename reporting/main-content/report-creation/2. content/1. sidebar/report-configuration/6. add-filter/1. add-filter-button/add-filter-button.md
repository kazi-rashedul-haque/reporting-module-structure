### Positive Use Cases:
1. User clicks `Add Filter` to open the filter modal:
   * Given the user is on the report customization form and no filters have been applied yet, the `Add Filter` button is enabled.
   * User clicks the `Add Filter` button, and the filter modal opens successfully.

2. User opens the filter modal:
   * The filter modal should open without any error.
   * The modal should display all the available filter options for the user to choose from.

3. User interacts with the filter form and applies a filter:
   * After the filter modal opens, the user can select filter criteria, apply the filter, and the system applies the filter to the report.

### Negative Use Cases:
1. User tries to click `Add Filter` after a filter is already applied:
   * After a filter has been applied and the `Clear` button is visible, the `Add Filter` button should still be enabled, but it should not cause the user to apply one or more filter again.

2. User tries to click `Add Filter` when the filter modal is already open:
   * User will not be able to click the `Add Filter` button when the `Filters` modal is already open.

### Edge Use Cases:
1. User rapidly clicks `Add Filter` multiple times:
   * The application should prevent multiple instances of the modal from opening simultaneously.
   * Only one modal should be displayed at any given time.

2. User applies multiple filters one after another:
   * The system should handle applying several filters sequentially and ensure the `Add Filter` button remains visible at the bottom right.

3. User interacts with different types of filters (e.g., dropdowns, checkboxes):
   * The filter modal should handle multiple filter types and should function seamlessly regardless of filter type.

### Accessibility Use Cases:
1. `Add Filter` button is focusable and accessible via keyboard navigation:
   * Users should be able to navigate to the `Add Filter` button using the Tab key.
   * The button should be focusable and clickable using the Enter key.

2. Screen readers announce the `Add Filter` button:
   * When using a screen reader, the `Add Filter` button should be properly announced with accessible text (e.g., `Add Filter`).
   * The screen reader should also announce the state (enabled/disabled) of the button.

3. Button should be properly labeled for accessibility:
   * Ensure the `Add Filter` button has an appropriate aria-label (e.g., aria-label=`Add Filter`).
   * Ensure the button is visually distinguishable (with sufficient contrast) and has clear textual content.