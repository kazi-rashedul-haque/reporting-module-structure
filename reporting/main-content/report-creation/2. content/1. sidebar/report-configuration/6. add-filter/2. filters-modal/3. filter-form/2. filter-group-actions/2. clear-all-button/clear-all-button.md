### Positive Use Cases:
1. Clear All Filters
   * User clicks `Clear All` and all filters (including nested filters) are removed or reset, leaving the UI in its initial/empty state.

2. Clear All with Single Filter
   * User clicks `Clear All` when only one filter is present; UI resets to default/empty filter row or blank state.

### Negative/Edge Use Cases:
1. Clear All with Unsaved Changes
   * User has filled filter rows but hasn’t saved/applied; clicks Clear All and system clears everything, possibly with a warning.

### Accessibility Use Cases:
1. Keyboard Accessibility: User can focus the button via keyboard and activate it via Enter/Space.
2. Screen Reader Accessibility: Button has proper labeling for accessibility tools.