**Title:** Verify favorite button accessibility and keyboard navigation

**Test Steps:**
1. Login to the workspace as an authenticated user.
2. Navigate to the Reporting page and open any report details.
3. Use Tab key to navigate to the Actions dropdown button.
4. Press Enter or Space to open the Actions dropdown.
5. Use Tab key to navigate to the favorite button within the dropdown.
6. Verify the favorite button receives proper focus indication.
7. Press Enter or Space to activate the favorite button.
8. Verify the favorite state changes correctly via keyboard interaction.
9. Test screen reader announcements for button state and tooltip text.
10. Verify ARIA labels and roles are properly implemented.
11. Test high contrast mode compatibility for visual indicators.
12. Verify focus management when dropdown closes after favorite action.

**Expected Result:**
* Favorite button is reachable via keyboard navigation within Actions dropdown
* Button receives clear and visible focus indicator when tabbed to
* Enter and Space keys successfully activate the favorite toggle functionality
* Screen readers properly announce button purpose and current state
* Screen readers announce state changes when favorite status is toggled
* ARIA labels accurately describe button function and current state
* High contrast mode displays button states clearly and distinguishably
* Focus management works correctly when dropdown closes after interaction
* All accessibility standards (WCAG 2.1 AA) are met for the favorite button
* Keyboard-only users can fully interact with favorite functionality