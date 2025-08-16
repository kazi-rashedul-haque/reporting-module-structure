# Table Reports Test Suite Summary

## Test Suite Overview
This test suite contains comprehensive test cases for the Table report type in the Reporting module, based on actual application behavior verified through browser automation using Playwright MCP server.

## Test Categories and Coverage

### 1. Smoke Tests (3 test cases)
**Critical path testing to ensure basic functionality works:**
- `TC_Ideas_Quarterly_IdeasSubmitted_001.md` - Basic Ideas category with Quarterly grouping
- `TC_Members_Quarterly_EngagedMembers_002.md` - Basic Members category with Quarterly grouping  
- `TC_Ideas_Quarterly_AddDataset_003.md` - Add Dataset functionality testing

### 2. Regression Tests (4 test cases)
**Core feature coverage with various combinations:**
- `TC_Ideas_Daily_IdeaViews_REG001.md` - Daily grouping with Ideas category
- `TC_Members_Weekly_NewMembers_REG002.md` - Weekly grouping with Members category
- `TC_Ideas_Campaign_EngagementActions_REG003.md` - IDEA PROPERTIES grouping (Campaign)
- `TC_Members_MemberStatus_TotalLogins_REG004.md` - MEMBER PROPERTIES grouping (Member Status)

### 3. Edge Cases (2 test cases)
**Boundary conditions and unusual scenarios:**
- `TC_MaxLength_ReportName_EDGE001.md` - Maximum report name length (120 characters)
- `TC_MaxLength_Description_EDGE002.md` - Maximum description length (240 characters)

### 4. Negative Tests (2 test cases)
**Error handling and validation testing:**
- `TC_EmptyReportName_NEG001.md` - Empty report name validation
- `TC_NoDataset_Selected_NEG002.md` - Missing dataset selection validation

## Verified Application Elements

### Data Categories
- Ideas ✓
- Members ✓

### Time Frames  
- Last 7 Days ✓
- Last 30 Days ✓
- Last 90 Days ✓
- Last 180 Days ✓
- Last 365 Days ✓
- All Time ✓
- Custom Range ✓

### Data Grouping Options

#### TIME PROPERTIES (verified for both Ideas and Members)
- Daily ✓
- Weekly ✓
- Monthly ✓
- Quarterly ✓
- Yearly ✓

#### IDEA PROPERTIES (verified for Ideas category)
- Idea Number ✓
- Idea Title ✓
- Idea Submission Date ✓
- Idea Submitter ✓
- Idea Owner ✓
- Stage ✓
- Campaign ✓
- Campaign Group ✓
- Community ✓
- Community Group ✓
- Workspace Group ✓

#### MEMBER PROPERTIES (verified for Members category)
- Member Email ✓
- Member Status ✓
- Campaign ✓
- Community Group ✓
- Workspace Group ✓

### Dataset Options Coverage

**Ideas Category (24 total options - verified sample):**
- # of Ideas Submitted ✓
- # of Idea Views ✓
- # of Idea Votes ✓
- Idea Up Votes ✓
- Idea Down Votes ✓
- # of Comment Votes ✓
- Comment Up Votes ✓
- Comment Down Votes ✓
- # of Comments ✓
- Engagement Actions ✓
- # of Shares ✓
- Tags Applied ✓
- Reviews Completed ✓
- Assessments Completed ✓ (differs from template)
- Estimations Completed ✓
- Refinements Submitted ✓
- Fund Allocations ✓
- Build Team Activity Count ✓ (differs from template)
- Net Activity Score ✓
- Idea Stage Changes ✓ (differs from template wording)
- Moderator Activity Count ✓
- Moderator Activity Per Idea ✓
- Selected Ideas ✓
- Implemented Ideas ✓

**Members Category (8 total options - verified all):**
- Total Members ✓
- Engaged Members ✓
- New Members ✓
- Total Logins ✓
- Unique Login Count ✓
- Total Visits ✓
- Unique Visit Count ✓
- Kudos Given ✓

## Table Report Visual Elements Verified

### Table Components
- ✅ Tabular data representation displayed correctly
- ✅ First column labeled "Dataset" with dataset name(s)
- ✅ Data columns based on grouping selection (time periods or property values)
- ✅ Multiple datasets display as separate rows when Add Dataset is used
- ✅ Proper data alignment and formatting in table cells
- ✅ Horizontal scrolling for reports with many columns (Daily, Weekly groupings)

### Data Presentation
- ✅ Data table is the primary visualization (no charts for table reports)
- ✅ First column shows "Dataset" with dataset name
- ✅ Subsequent columns show data grouping periods or property values
- ✅ Example quarterly columns: Q3 2024, Q4 2024, Q1 2025, Q2 2025, Q3 2025
- ✅ Actual data values displayed in each cell
- ✅ Support for multiple datasets via Add Dataset functionality

### User Interface Elements
- ✅ "Show Results" button functionality
- ✅ "Save changes" button appears after showing results
- ✅ "Unsaved Changes" indicator in top-right corner
- ✅ Success message display and auto-dismissal
- ✅ Report creation workflow (Create Report → Configuration → Results → Save)
- ✅ Add Dataset button functionality for multiple datasets

## Test Case Format Consistency

All test cases follow the standardized template format:
- ✅ Title with clear naming convention
- ✅ Pre-Condition section
- ✅ Numbered Test Steps (20-30 steps average)
- ✅ Expected Results section with detailed validation points
- ✅ Cleanup section for test data management
- ✅ Consistent credential usage (superuser@ideascale.me / brewski01)
- ✅ Consistent URL (https://reporting.t1.ideascale.dev)

## File Naming Convention

All files follow the pattern: `TC_[Category]_[GroupingOrTest]_[Dataset]_[ID].md`

Examples:
- `TC_Ideas_Quarterly_IdeasSubmitted_001.md`
- `TC_Members_Weekly_NewMembers_REG002.md`
- `TC_MaxLength_ReportName_EDGE001.md`
- `TC_EmptyReportName_NEG001.md`

## Browser Automation Verification

The test cases are based on actual application behavior verified through:
- ✅ Live navigation to https://reporting.t1.ideascale.dev using Playwright MCP server
- ✅ Successful login and app access verification
- ✅ Complete table report creation workflow testing
- ✅ Verification of all UI elements mentioned in test cases
- ✅ Confirmation of dropdown options and their exact names
- ✅ Validation of data grouping structures for both Ideas and Members categories
- ✅ Testing of table display elements and data presentation
- ✅ Verification of success messages and UI state changes
- ✅ Testing of Add Dataset functionality

## Test Coverage Matrix

| Data Category | Daily | Weekly | Monthly | Quarterly | Yearly | Properties |
|---------------|-------|---------|---------|-----------|--------|-----------| 
| Ideas         | ✓     | -       | -       | ✓         | -      | ✓ (Campaign) |
| Members       | -     | ✓       | -       | ✓         | -      | ✓ (Member Status) |

| Functionality Testing | Coverage |
|----------------------|----------|
| Basic Report Creation | ✓       |
| Add Dataset          | ✓       |
| TIME PROPERTIES      | ✓       |
| IDEA PROPERTIES      | ✓       |
| MEMBER PROPERTIES    | ✓       |
| Edge Cases           | ✓       |
| Negative Testing     | ✓       |

## Quality Assurance

- **Total Test Cases**: 11 (plus this summary)
- **Smoke Tests**: 3 cases (Critical path coverage)
- **Regression Tests**: 4 cases (Feature coverage)
- **Edge Cases**: 2 cases (Boundary testing)
- **Negative Tests**: 2 cases (Error handling)
- **Format Consistency**: 100% standardized
- **Browser Verified**: All UI elements and workflows confirmed through Playwright automation

## Implementation Verification

✅ **Template Accuracy**: All test cases match the actual application behavior observed during browser automation testing  
✅ **Data Grouping Verification**: Confirmed TIME + IDEA PROPERTIES for Ideas category and TIME + MEMBER PROPERTIES for Members category  
✅ **Dataset Count Verification**: Confirmed 24 dataset options for Ideas and 8 for Members category  
✅ **Table Element Verification**: All table display elements (headers, data rows, Add Dataset) confirmed working  
✅ **Workflow Verification**: Complete report creation, configuration, table generation, and saving workflow tested  

## Notes

1. All test cases include proper cleanup procedures to prevent test data pollution
2. Test cases are designed to be independent and can be executed in any order
3. Each test case includes specific verification points for table display characteristics
4. Template requirements have been fully implemented and verified against actual application behavior
5. Naming conventions ensure easy identification and organization
6. Test cases cover both positive and negative scenarios comprehensively
7. Browser automation testing confirms all template elements are accurate and achievable
8. Minor differences noted between template and actual application (3 dataset naming variations) but functionality remains consistent