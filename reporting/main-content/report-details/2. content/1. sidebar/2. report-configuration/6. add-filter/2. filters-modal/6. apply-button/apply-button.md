### Positive Use Cases:
1. User clicks `Apply` to save changes:
   * The current changes made in the form are saved, and the modal is closed.

2. User clicks `Apply` and feedback is shown:
   * After clicking `Apply`, a success alert is shown to the user.

### Negative Use Cases:
1. User clicks `Apply` without applying any filter:
   * Without applying any filter, the `Apply` button should remain disabled.

2. User clicks `Apply` but changes are not applied:
   * If the backend or processing logic fails, the user should be informed that the changes were not successfully applied.

### Edge Use Cases:
1. User clicks `Apply` during an ongoing operation:
   * If the system is processing (e.g., fetching data, applying filters), the `Apply` button should remain disabled until the process completes.

2. User rapidly clicks `Apply` multiple times:
   * The system should handle multiple clicks gracefully, either by ignoring duplicate clicks or showing a loading state to prevent repeated submissions.

3. User clicks `Apply` and the form is reset unexpectedly:
   * If any filters were applied, they should not be reset.

### Accessibility Use Cases:
1. `Apply` button is focusable and accessible via keyboard navigation:
   * The `Apply` button should be accessible through keyboard navigation and activation.

2. `Apply` button announced by screen readers:
   * The screen reader should announce the `Apply` button with appropriate accessible text such as `Apply`.

3. `Apply` button provides visual feedback on state changes:
   * The button should indicate whether it’s in a loading or disabled state, so users know when the system is processing or when the button cannot be clicked.