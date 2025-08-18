# Generalized Pagination Test Cases

This directory contains pagination test cases that can be used for both **Dashboard List** and **Report List** components by replacing template parameters.

## Usage

### Template Parameters

When using these test cases, replace the following parameters based on your context:

| Parameter | Dashboard Context | Report Context |
|-----------|------------------|----------------|
| `{ITEM_TYPE}` | dashboard | report |
| `{ITEM_TYPE_PLURAL}` | dashboards | reports |
| `{ITEM_TYPE_PLURAL_CAPITALIZED}` | Dashboards | Reports |
| `{PAGE_NAME}` | Dashboard List | Reports |

### Example Substitutions

**For Dashboard List pagination:**
- `{ITEM_TYPE}` → dashboard
- `{ITEM_TYPE_PLURAL}` → dashboards  
- `{ITEM_TYPE_PLURAL_CAPITALIZED}` → Dashboards
- `{PAGE_NAME}` → Dashboard List

**For Report List pagination:**
- `{ITEM_TYPE}` → report
- `{ITEM_TYPE_PLURAL}` → reports
- `{ITEM_TYPE_PLURAL_CAPITALIZED}` → Reports  
- `{PAGE_NAME}` → Reports

### Available Test Cases

1. **Verify pagination appears when {ITEM_TYPE_PLURAL} exceed 10 items.md**
2. **Verify pagination does not appear with 10 or fewer {ITEM_TYPE_PLURAL}.md**
3. **Verify next page navigation functionality.md**
4. **Verify previous page navigation functionality.md**
5. **Verify next button is disabled on last page.md**
6. **Verify previous button is disabled on first page.md**
7. **Verify pagination total count display functionality.md**
8. **Verify pagination accessibility compliance.md**

### Implementation Steps

1. **Copy template files** to your specific component test directory
2. **Replace parameters** with context-specific values using find-and-replace
3. **Review test steps** for any additional context-specific requirements
4. **Execute tests** in your specific environment

### Example Implementation

For Dashboard List:
```bash
# Copy files to dashboard list test directory
cp pagination-testcases/* ../main-content/dashboard-list/content/dashboard-table/pagination-testcases/

# Replace parameters (using your preferred text editor or script)
find ../main-content/dashboard-list/content/dashboard-table/pagination-testcases/ -name "*.md" -exec sed -i 's/{ITEM_TYPE_PLURAL_CAPITALIZED}/Dashboards/g' {} \;
find ../main-content/dashboard-list/content/dashboard-table/pagination-testcases/ -name "*.md" -exec sed -i 's/{ITEM_TYPE_PLURAL}/dashboards/g' {} \;
find ../main-content/dashboard-list/content/dashboard-table/pagination-testcases/ -name "*.md" -exec sed -i 's/{ITEM_TYPE}/dashboard/g' {} \;
find ../main-content/dashboard-list/content/dashboard-table/pagination-testcases/ -name "*.md" -exec sed -i 's/{PAGE_NAME}/Dashboard List/g' {} \;
```

This approach ensures consistency across all pagination implementations while maintaining component-specific context.