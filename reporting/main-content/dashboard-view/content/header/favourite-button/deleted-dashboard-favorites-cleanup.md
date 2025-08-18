**Title**: Deleted Dashboard Favorites Cleanup

**Description**: Verify favorite references are cleaned up when dashboard is deleted
**Pre-Condition**: Favorited dashboard that can be deleted
**Test Steps**:
1. Favorite a dashboard
2. Delete the dashboard
3. Check favorites list and references
**Expected Result**:
- Deleted dashboard is removed from favorites list
- No broken references remain
- Favorites list displays correctly without deleted items
- System handles cleanup gracefully