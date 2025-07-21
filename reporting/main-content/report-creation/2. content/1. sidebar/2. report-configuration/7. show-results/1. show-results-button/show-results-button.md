1. **Disabled by Default**
   * Condition: No changes have been made to the report configuration since the last save or since the report was loaded.
   * Behavior:
     - Button is disabled (disabled={isEmpty(dirtyFields)}).
     - Greyed out visually.
     - User cannot trigger report generation.

2. **Enabled when Configuration is Modified**
   * Condition: User makes any change in the report configuration (e.g., changes grouping, dataset, axis, etc.).
   * Behavior:
     - Button becomes enabled (disabled={false}).
     - Primary color styling applied (visually stands out).
     - User can click to refresh/generate a report based on the latest configuration.

3. **Submitting – Shows Loading State**
   * Condition: User clicks `Show Results` while enabled.
   * Behavior:
     - The button may show a loading spinner.
     - Prevents multiple submissions.

4. **Disabled After Click**
   * Condition: After `Show Results` is clicked, until the new results are loaded.
   * Behavior: Button is disabled again (prevents double-click or spamming).

5. **Remains Disabled if No Change is Detected**
   * Condition: If a user tries to click `Show Results` without making any changes.
   * Behavior: Nothing happens.

### Test Case Ideas

**Positive**:
1. Changing any configuration enables `Show Results` and shows `Save changes`.
2. Clicking `Show Results` generates new results.
3. Clicking `Save changes` persists configuration.
4. `Show Results` disabled when there are no changes made.

**Negative/Edge**:
1. Trying to click `Show Results` with no changes (remains disabled).
2. Saving changes twice rapidly (second is ignored).
3. `Save changes` hidden for system-generated reports.
4. Rapid toggling between changes and save actions.