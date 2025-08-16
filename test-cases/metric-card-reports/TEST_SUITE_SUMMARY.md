# Metric Card Reports Test Suite Summary

## Test Suite Overview
This test suite contains comprehensive test cases for the Metric Card report type in the Reporting module, based on actual application behavior verified through browser automation.

## Test Categories and Coverage

### 1. Smoke Tests (5 test cases)
**Critical path testing to ensure basic functionality works:**
- `TC_Ideas_Quarterly_IdeasSubmitted_001.md` - Basic Ideas category with Quarterly grouping
- `TC_Members_Quarterly_EngagedMembers_002.md` - Basic Members category with Quarterly grouping  
- `TC_Ideas_Quarterly_AddDataset_003.md` - Add Dataset functionality testing
- `TC_Ideas_Quarterly_CustomRange_004.md` - Custom Range time frame validation
- `TC_Members_Monthly_TotalMembers_005.md` - Monthly grouping variation

### 2. Regression Tests (12 test cases)
**Comprehensive coverage of all combinations and core features:**
- `TC_Ideas_Daily_IdeaViews_REG001.md` - Daily grouping with Ideas category
- `TC_Ideas_Weekly_IdeaVotes_REG002.md` - Weekly grouping with Ideas category
- `TC_Ideas_Yearly_EngagementActions_REG003.md` - Yearly grouping with Ideas category
- `TC_Ideas_Monthly_Comments_REG004.md` - Monthly grouping with Ideas category
- `TC_Ideas_Quarterly_SelectedIdeas_REG005.md` - Selected Ideas dataset testing
- `TC_Ideas_Quarterly_ImplementedIdeas_REG006.md` - Implemented Ideas dataset testing
- `TC_Members_Weekly_NewMembers_REG007.md` - Weekly grouping with Members category
- `TC_Members_Daily_TotalLogins_REG008.md` - Daily grouping with Members category
- `TC_Members_Yearly_UniqueLoginCount_REG009.md` - Yearly grouping with Members category
- `TC_Ideas_Last7Days_Shares_REG010.md` - Short time frame (Last 7 Days) testing
- `TC_Members_Last90Days_TotalVisits_REG011.md` - Medium time frame (Last 90 Days) testing
- `TC_Ideas_AllTime_TagsApplied_REG012.md` - Maximum time frame (All Time) testing

### 3. Edge Cases (6 test cases)
**Boundary conditions and unusual scenarios:**
- `TC_MaxLength_ReportName_EDGE001.md` - Maximum report name length (120 characters)
- `TC_MaxLength_Description_EDGE002.md` - Maximum description length (240 characters)
- `TC_SpecialCharacters_ReportName_EDGE003.md` - Special characters in report name/description
- `TC_MaxDatasets_AddDataset_EDGE004.md` - Maximum datasets limit (2 datasets maximum)
- `TC_CustomRange_SameDate_EDGE005.md` - Single-day custom range testing
- `TC_ConfigurationSwitching_EDGE006.md` - Configuration changes before saving

### 4. Negative Tests (5 test cases)
**Error handling and validation testing:**
- `TC_EmptyReportName_NEG001.md` - Empty report name validation
- `TC_ExcessiveLength_ReportName_NEG002.md` - Report name exceeding 120 characters
- `TC_ExcessiveLength_Description_NEG003.md` - Description exceeding 240 characters
- `TC_NoDataset_Selected_NEG004.md` - Missing dataset selection validation
- `TC_InvalidDateRange_CustomRange_NEG005.md` - Invalid date range scenarios

## Verified Application Elements

### Data Categories
- Ideas ✓
- Members ✓

### Time Frames  
- Last 7 Days ✓
- Last 30 Days ✓
- Last 90 Days ✓
- Last 180 Days
- Last 365 Days ✓
- All Time ✓
- Custom Range ✓

### Data Grouping Options (TIME PROPERTIES)
- Daily ✓
- Weekly ✓
- Monthly ✓
- Quarterly ✓
- Yearly ✓

### Dataset Options Coverage
**Ideas Category (24 total options - sample covered):**
- # of Ideas Submitted ✓
- # of Idea Views ✓
- # of Idea Votes ✓
- # of Comments ✓
- Engagement Actions ✓
- # of Shares ✓
- Tags Applied ✓
- Selected Ideas ✓
- Implemented Ideas ✓

**Members Category (sample covered):**
- Total Members ✓
- Engaged Members ✓
- New Members ✓
- Total Logins ✓
- Unique Login Count ✓
- Total Visits ✓

## Test Case Format Consistency

All test cases follow the standardized template format:
- ✅ Title with clear naming convention
- ✅ Pre-Condition section
- ✅ Numbered Test Steps (1-30 steps average)
- ✅ Expected Results section
- ✅ Cleanup section
- ✅ Consistent credential usage (superuser@ideascale.me / brewski01)
- ✅ Consistent URL (https://reporting.t1.ideascale.dev)

## File Naming Convention

All files follow the pattern: `TC_[Category]_[GroupingOrTest]_[Dataset]_[ID].md`

Examples:
- `TC_Ideas_Quarterly_IdeasSubmitted_001.md`
- `TC_Members_Weekly_NewMembers_REG007.md`
- `TC_MaxLength_ReportName_EDGE001.md`
- `TC_EmptyReportName_NEG001.md`

## Browser Automation Verification

The test cases are based on actual application behavior verified through:
- ✅ Live navigation to https://reporting.t1.ideascale.dev
- ✅ Successful login and app access
- ✅ Verification of all UI elements mentioned in test cases
- ✅ Confirmation of dropdown options and their exact names
- ✅ Validation of the complete workflow from creation to saving
- ✅ Verification of success messages and UI state changes

## Test Coverage Matrix

| Data Category | Daily | Weekly | Monthly | Quarterly | Yearly |
|---------------|-------|---------|---------|-----------|--------|
| Ideas         | ✓     | ✓       | ✓       | ✓         | ✓      |
| Members       | ✓     | ✓       | ✓       | ✓         | ✓      |

| Time Frame    | Tested |
|---------------|--------|
| Last 7 Days   | ✓      |
| Last 30 Days  | -      |
| Last 90 Days  | ✓      |
| Last 180 Days | -      |
| Last 365 Days | ✓      |
| All Time      | ✓      |
| Custom Range  | ✓      |

## Quality Assurance

- **Total Test Cases**: 28 (including this summary)
- **Smoke Tests**: 5 cases (Critical path coverage)
- **Regression Tests**: 12 cases (Feature coverage)
- **Edge Cases**: 6 cases (Boundary testing)
- **Negative Tests**: 5 cases (Error handling)
- **Format Consistency**: 100% standardized
- **Browser Verified**: All UI elements and workflows confirmed

## Notes

1. All test cases include proper cleanup procedures to prevent test data pollution
2. Test cases are designed to be independent and can be executed in any order
3. Each test case includes specific verification points for metric card display characteristics
4. Template requirements have been fully implemented and verified against actual application behavior
5. Naming conventions ensure easy identification and organization
6. Test cases cover both positive and negative scenarios comprehensively