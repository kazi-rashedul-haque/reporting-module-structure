1. **Hidden by Default**
   * Condition: When there are no unsaved changes (unsavedChanges is false).
   * Behavior: Button is not rendered.

2. **Shown when Unsaved Changes exist**
   * Condition: There are unsaved changes in the configuration, and the report is not system-generated.
   * Behavior: Button appears with `Save changes` label and outline styling.

3. **Save Changes in the Header**
   * Condition: On the right-side header, an `Unsaved Changes` dropdown appears after `Show Results` is clicked, offering another way to save.
   * Behavior: User can open the dropdown and click `Save changes`.

4. **Save Button Disabled or Shows Loading**
   * Condition: While saving is in progress.
   * Behavior: Save button shows loading state, is disabled.

5. **After Save – Button Disappears**
   * Condition: Once changes are successfully saved.
   * Behavior:
     - `Save changes` button disappears from both the UI and the dropdown.
     - `Unsaved Changes` dropdown is removed.