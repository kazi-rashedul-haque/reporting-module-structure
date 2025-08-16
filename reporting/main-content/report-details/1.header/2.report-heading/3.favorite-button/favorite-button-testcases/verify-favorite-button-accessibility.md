**Title:** Verify favorite button accessibility features on report details page

**Pre-conditions:**
* At least one report exists in the report list

**Test Steps:**
1. Login to the workspace as an authenticated user.
2. Navigate to the Reporting page.
3. Select a report that is not favorited and open its details page.
4. Use Tab key to navigate to the favorite button.
5. Verify the button receives proper keyboard focus with visible focus indicator.
6. Verify the button has appropriate aria-label or accessible name describing its current state.
7. Press Enter or Space key to activate the favorite button.
8. Verify the button toggles to favorited state and focus remains on the button.
9. Verify the accessible name updates to reflect the new state.
10. Continue tabbing to ensure focus moves to the next focusable element properly.
11. Use Shift+Tab to navigate back to the favorite button.
12. Press Enter or Space key again to remove from favorites.
13. Verify the button state changes and accessible name updates accordingly.
14. Test with screen reader (if available) to ensure proper announcement of button state and changes. [Not supported in Playwright - use manual verification or accessibility testing tools like axe-core]

**Playwright Compatibility:** Most accessibility tests are supported. Keyboard navigation, focus management, and ARIA attributes can be automated. Screen reader testing requires manual verification or axe-core integration for automated accessibility auditing.

**Expected Result:**
* Favorite button is keyboard accessible via Tab navigation
* Button shows clear visual focus indicator when focused
* Button can be activated using Enter or Space key
* Button has appropriate aria-label or accessible name (e.g., "Add to Favorites" or "Remove from Favorites")
* Accessible name updates immediately when button state changes
* Focus management works properly when toggling favorite state
* Screen reader announces button state and changes clearly [Manual verification required]
* Button meets WCAG accessibility guidelines for interactive elements
* No keyboard traps or focus issues around the favorite button
* Color contrast meets accessibility standards for both icon states