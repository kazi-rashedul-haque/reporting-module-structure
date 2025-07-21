### Positive Use Cases:
1. Delete a Filter Row
   * User clicks the delete button for a filter row; that specific row is immediately removed from the filter list.

2. Delete Multiple Filter Rows
   * User deletes more than one filter row in any order; each targeted row is removed and the filter list updates accordingly.

3. Clear All Filters Using Delete Buttons
   * User clicks delete on each filter row one by one until all are removed.

### Negative/Edge Use Cases:
1. Delete Last Remaining Filter Row
   * User attempts to delete the only remaining filter row; system allows deletion of the last row.

2. Delete During Edit
   * User is editing filter fields in a row and clicks delete; the row is removed without error or leaving UI artifacts.

### Accessibility Use Cases:
1. Keyboard Accessibility
   * User can navigate to the delete button using Tab/Shift+Tab and activate it via Enter/Space.

2. Screen Reader Accessibility
   * Delete button has proper labeling (via aria-label or title) so screen readers describe its function.
