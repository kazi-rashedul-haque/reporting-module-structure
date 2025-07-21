### Positive Use Cases:
1. Add a New Filter
   * User clicks the `Add Filter` button; a new filter row is added to the filter list.

2. Add Multiple Filters Sequentially
   * User clicks the `Add Filter` button multiple times to add multiple filter rows in sequence.

3. Add Filter When No Filters Are Present
   * User clicks `Add Filter` when there are no existing filters; the first filter row is added.

4. Add Filter After Deleting Other Filters
   * User deletes one or more filters and then clicks the `Add Filter` button to add a new filter row.

5. Add Filter After Applying Filters
   * User applies the existing filters and later clicks `Add Filter` to add a filter; the new filter is added without affecting previously applied filters.

6. Add Filter With Pre-existing Logical Operators
   * When a logical operator (e.g., AND, OR) is already selected, the user adds a new filter, which appropriately reflects the operator choice.

7. Add Filter in Different Sections
   * User can add filters in different sections, creating a logical structure where different filter groups are maintained.

### Negative/Edge Use Cases:
1. Add Filter When Conditions Are Not Fully Specified
   * User attempts to add a filter without specifying the necessary values (e.g., missing condition or type). The system should either allow adding empty filters or display an error prompting the user to complete the condition.

2. Add Filter with Invalid Filter Conditions
   * User adds a filter, but the condition selected (e.g., Equals) doesn’t align with the selected type. A validation message or error appears, indicating the mismatch.

### Accessibility Use Cases:
1. Keyboard Navigation: User can focus the Add Filter button using the Tab key and activate it using Enter or Space.
2. Screen Reader Accessibility: The Add Filter button is labeled properly for screen readers, allowing visually impaired users to know the action of the button.