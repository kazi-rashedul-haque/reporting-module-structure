# TC_MANAGE_DASHBOARDS_EDGE_003: Multiple Dashboard Management Sessions

**Description**: Verify behavior when management is accessed from multiple sessions
**Pre-Condition**: Same user logged in multiple browser sessions
**Test Steps**:
1. Open dashboard management from multiple sessions
2. Verify concurrent access handling
**Expected Result**:
- Multiple sessions can access management view
- No conflicts between concurrent sessions
- Changes made in one session are reflected in others
- Consistent behavior across all sessions