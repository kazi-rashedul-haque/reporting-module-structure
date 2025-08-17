# TC_DELETE_MODAL_ACC_003: Focus Management

**Description**: Verify proper focus management in modal

**Pre-Condition**: Delete modal is open

**Test Steps**:
1. Open modal and observe initial focus
2. Tab through all elements
3. Close modal and observe focus return

**Expected Result**:
- Focus starts on the first actionable element (Cancel or Delete)
- Focus is trapped within modal
- Focus returns to delete trigger button when modal closes
- Focus indicator is visible throughout