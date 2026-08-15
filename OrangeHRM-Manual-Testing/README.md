# OrangeHRM Manual Testing

## Application
[OrangeHRM Demo](https://opensource-demo.orangehrmlive.com/web/index.php/auth/login)

## Module Tested
- Login

> Note: Currently only the Login module is covered. Dashboard, PIM, and Leave modules are planned for future additions.

## Documents
- [Test Scenarios](./OrangeHRM_completed.xlsx) — sheet: `Test Scenerio`
- [Decision Table](./OrangeHRM_completed.xlsx) — sheet: `Decision Details`
- [Test Cases](./OrangeHRM_completed.xlsx) — sheet: `Test Cases`

## Approach
- **Technique used:** Decision Table Testing — all valid/invalid/blank combinations of Username and Password were mapped and tested (9 test cases).
- **Test case format:** SR No, Test Case ID, Scenario Title, Test Case Title, Pre-conditions, Steps, Test Data, Actual Result, Expected Result, Status.

## Scope Note
The public OrangeHRM demo site does not expose a self-service Registration page. The Register Page test cases in this repo are written against a **generic registration form** as a demonstration of standard field-validation testing practice (mandatory fields, format checks, duplicate handling, password confirmation) — not against a live OrangeHRM feature.

## Tools
- Excel (manual test case documentation)

## Status
✅ Login — 9/9 test cases executed, all passing
📝 Register (generic form) — 17/17 test cases documented as a reference example
