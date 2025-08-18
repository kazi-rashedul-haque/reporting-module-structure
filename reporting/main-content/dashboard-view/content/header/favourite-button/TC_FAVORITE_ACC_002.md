# TC_FAVORITE_ACC_002: Screen Reader Support

**Description**: Verify favorite button is compatible with screen readers
**Pre-Condition**: Screen reader is active
**Test Steps**:
1. Navigate to favorite button with screen reader
2. Listen to button announcement
3. Activate button and listen to state change announcement
**Expected Result**:
- Button is announced with current state ("Add to Favorites" or "Remove from Favorites")
- Button role is properly announced
- State changes are announced when button is activated
- Instructions are clear and actionable