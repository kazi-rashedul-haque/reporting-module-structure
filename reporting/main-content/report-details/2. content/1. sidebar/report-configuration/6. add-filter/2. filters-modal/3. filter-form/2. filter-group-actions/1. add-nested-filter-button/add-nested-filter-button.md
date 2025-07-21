### Positive Use Cases:
1. Add a Nested Filter
   * User clicks `Add Nested Filter` and a new nested filter row is added under the current filter/group.

2. Add Multiple Nested Filters
   * User clicks `Add Nested Filter` multiple times; each click adds another nested filter under the same parent.

3. Add Nested Filter With Pre-existing Filters
   * User adds a nested filter when there are already existing parent/child filters; nesting works as expected.

4. Add Nested Filter in Different Groups
   * User adds nested filters to different filter groups, ensuring each group nests independently.

### Negative/Edge Use Cases:
1. Exceed Maximum Nesting Level
   * Users can add as many nested filters as they want.

2. Add Nested Filter When Parent is Incomplete
   * User tries to add a nested filter when the parent filter row is not fully filled; appropriate validation or behavior is triggered.

3. Rapid/Multi-click
   * User rapidly clicks Add Nested Filter; app correctly adds only the allowed number of filters and maintains performance.

### Accessibility Use Cases:
1. Keyboard Accessibility: User can focus the button via keyboard and add a nested filter with Enter/Space.
2. Screen Reader Accessibility: Button has descriptive text/aria-label for screen readers.