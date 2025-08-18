**Title:** Verify Clear All button removes all configured filters and resets form to initial state

**Pre-Condition:**
1. User is logged into the reporting application
2. User is on the report creation page with completed basic configuration
3. Add Filter modal is open
4. Multiple filters are configured with various conditions and nested filters

**Test Steps:**
1. Configure a complex filter structure:
   - Main WHERE filter with complete configuration
   - Multiple nested filters with different logical operators (AND/OR)
   - Various operand types and values
2. Click the "Clear All" button
3. Observe the filter form state
4. Verify all filter configurations are removed
5. Test Clear All with single filter configuration
6. Test Clear All when no filters exist

**Expected Results:**
1. "Clear All" button is visible and properly labeled
2. Clicking "Clear All" removes all configured filters:
   - Main WHERE filter is reset to default state
   - All nested filters are completely removed
   - Form returns to initial empty state
3. After clearing, form displays:
   - Single WHERE filter row with default settings
   - Left operand shows "Select" placeholder
   - Comparison operator shows default value
   - Right operand shows appropriate default input type
   - No nested filter rows remain
4. Clear All functionality:
   - Works consistently with any filter configuration complexity
   - Action is immediate and irreversible
   - Does not close the modal (user remains in filter editing mode)
5. When no filters exist:
   - Clear All button is either disabled or has no effect
   - Form remains in default state
6. Filter form maintains proper structure and functionality after clearing