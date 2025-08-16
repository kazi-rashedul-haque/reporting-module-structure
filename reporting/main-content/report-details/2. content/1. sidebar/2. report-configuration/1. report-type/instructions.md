# Report Type Test Cases Instructions

## Overview

This document outlines the standardized structure and requirements for test cases across all report types in the Ideascale Reporting module. Each report type follows identical patterns to ensure consistency and maintainability.

## Report Types

The following report types are supported and must have corresponding test cases:

- **Line** - Line chart visualizations
- **Bar** - Vertical bar chart visualizations  
- **Horizontal Bar** - Horizontal bar chart visualizations
- **Dual Axis** - Charts with two Y-axes for different data scales
- **Metric Card** - Single metric display cards
- **Donut** - Donut/pie chart visualizations
- **Table** - Tabular data display (no chart visualization)

## Folder Structure

```
1. report-type/
├── 1. line/
│   ├── use-cases.md
│   └── line-testcases/
│       ├── Verify line chart radio button selection functionality.md
│       ├── Verify Data Category dropdown options display correctly.md
│       ├── Verify Time Frame dropdown displays data metrics correctly.md
│       ├── Verify Add Dataset functionality for dual Y Axis.md
│       ├── Verify Show Results button behavior with incomplete configuration.md
│       ├── Verify line chart tooltip display on hover.md
│       └── Verify Accessibility compliance in line chart report type selection.md
├── 2. bar/
│   ├── use-cases.md
│   └── bar-testcases/
│       └── [7 test case files following same pattern]
├── 3. horizontal-bar/
│   ├── use-cases.md
│   └── horizontal-bar-testcases/
│       └── [7 test case files following same pattern]
├── 4. dual-axis/
│   ├── use-cases.md
│   └── dual-axis-testcases/
│       └── [7 test case files following same pattern]
├── 5. metric-card/
│   ├── use-cases.md
│   └── metric-card-testcases/
│       └── [7 test case files following same pattern]
├── 6. donut/
│   ├── use-cases.md
│   └── donut-testcases/
│       └── [7 test case files following same pattern]
├── 7. table/
│   ├── use-cases.md
│   └── table-testcases/
│       └── [7 test case files following same pattern]
└── instructions.md (this file)
```

## Required Test Cases

Each report type folder **MUST** contain exactly **7 test case files** covering the following standardized scenarios:

### 1. Radio Button Selection Functionality
- **File naming pattern**: `Verify {report-type} radio button selection functionality.md`
- **Purpose**: Tests the basic selection of the report type from the Report Type group
- **Coverage**: Radio button interaction, visual state changes, configuration options appearance

### 2. Data Category Dropdown Functionality  
- **File naming pattern**: `Verify Data Category dropdown options display correctly.md`
- **Purpose**: Tests the Data Category selection functionality
- **Coverage**: Dropdown/combobox interaction, option display, selection persistence

### 3. Time Frame Selection Functionality
- **File naming pattern**: `Verify Time Frame dropdown displays data metrics correctly.md`
- **Purpose**: Tests time frame selection and its impact on data
- **Coverage**: Time frame options, selection behavior, data refresh

### 4. Add Dataset Functionality
- **File naming pattern**: `Verify Add Dataset functionality for {dual Y Axis|multiple datasets}.md`
- **Purpose**: Tests the ability to add additional datasets to reports
- **Coverage**: Add Dataset button, multiple dataset configuration, data combination

### 5. Show Results Button Validation
- **File naming pattern**: `Verify Show Results button behavior with incomplete configuration.md`
- **Purpose**: Tests form validation and submission behavior
- **Coverage**: Button state management, validation logic, error handling

### 6. Interactive Elements (Tooltips/Hover)
- **File naming pattern**: `Verify {report-type} tooltip display on hover.md`
- **Purpose**: Tests interactive elements and user feedback
- **Coverage**: Hover states, tooltip content, interaction responsiveness

### 7. Accessibility Compliance
- **File naming pattern**: `Verify Accessibility compliance in {report-type} report type selection.md`
- **Purpose**: Tests comprehensive accessibility requirements
- **Coverage**: Keyboard navigation, screen reader compatibility, ARIA compliance, visual accessibility

## Test Case Requirements

### Content Structure
Each test case file must include:
- **Title**: Clear, descriptive test case name
- **Pre-conditions**: Required setup conditions
- **Test Steps**: Numbered, specific steps with element references
- **Expected Result**: Detailed expected outcomes with verifiable criteria

### Playwright Compatibility
- Use specific element selectors and references from actual UI
- Include Playwright compatibility annotations where needed
- Mark unsupported features with alternatives: `[Not supported in Playwright – use alternative]`
- Structure test steps for automation conversion

### Accessibility Testing Format
Accessibility test cases must follow the structured format with:
- Horizontal rule separators (`---`)
- Detailed keyboard navigation expectations
- Screen reader compliance requirements
- WCAG AA compliance criteria

## Naming Conventions

### Folder Names
- Pattern: `{number}. {report-type}/`
- Examples: `1. line/`, `6. donut/`, `7. table/`

### Test Case Folder Names  
- Pattern: `{report-type}-testcases/`
- Examples: `line-testcases/`, `donut-testcases/`, `table-testcases/`

### Test Case File Names
- Must match the test case title exactly
- Use descriptive, action-oriented names
- Include report type name where applicable
- End with `.md` extension

## Reusability Rules

### Standardization
- All report types follow identical test case patterns
- Only report-type-specific terminology should differ
- UI element interactions remain consistent across types
- Expected results follow the same verification patterns

### Customization Guidelines
When adapting test cases for different report types:

1. **Replace report type names** in titles and content
2. **Update chart-specific terminology** (e.g., "line chart tooltip" vs "donut chart segments")
3. **Maintain identical test step structure** and numbering
4. **Keep accessibility requirements consistent** across all types
5. **Preserve Playwright compatibility annotations**

### Quality Assurance
- Each report type must have exactly 7 test cases
- Test case file names must match internal titles
- All test cases must be executable manually
- All test cases must provide clear automation guidance

## Maintenance

### Adding New Report Types
1. Create numbered folder following pattern: `{next-number}. {report-type}/`
2. Add `use-cases.md` file with report type requirements
3. Create `{report-type}-testcases/` subfolder
4. Generate 7 test cases following the standardized patterns
5. Update this instructions file to include the new report type

### Updating Existing Test Cases
- Maintain consistency across all report types when making changes
- Update all affected report types simultaneously
- Preserve the 7-test-case requirement
- Ensure Playwright compatibility is maintained

---

**Note**: This standardized approach ensures consistency, maintainability, and efficient automation conversion across all report types in the Ideascale Reporting module.