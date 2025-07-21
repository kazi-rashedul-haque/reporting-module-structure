Button Label: `Unsaved Changes`
Trigger: Displayed in the top-right corner when the user clicks `Show Results` after modifying the report configuration (e.g., changing report type, axis, or dataset).

**Behavior**:
**Save Changes Button**:
- When selected, the current report configuration is saved.
- A success alert is shown to confirm the update.

**Unsaved Changes Warning Modal**:
Trigger: If the user attempts to navigate away from the report page (e.g., using the back button) without saving the recent changes.

**Modal Content**:
Title: `You have unsaved changes`
Description: Click `Continue Editing` to keep editing or `Discard Changes` to abandon changes.

**Actionable Buttons**:
1. Continue Editing:
   * Closes the modal and allows the user to continue editing.
   * No changes are discarded.

2. Discard Changes:
   * Confirms abandonment of all unsaved changes.
   * Navigation proceeds and previous report state is retained.