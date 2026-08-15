# SauceDemo Manual Testing

## Application
[SauceDemo](https://www.saucedemo.com/) — a sample e-commerce site built for QA practice.

## Flow Tested
Full end-to-end flow: **Login → Products → Cart → Checkout → Logout**

## Documents
- [Test Scenario & Test Cases](./SauceDemo_TestCases.xlsx) — sheets: `Project Details`, `Test Scenerio`, `Test Cases`
- [Bug Report](./SauceDemo_Bug_Report.xlsx)
- [Test Summary Report](./SauceDemo_Test_Summary_Report.xlsx)

## Scope
- **21 formal test cases** executed with the `standard_user` account, covering:
  - Login (valid/invalid credentials, locked-out user, blank fields) — 5 TCs
  - Products page (listing, add/remove to cart, sorting) — 7 TCs
  - Checkout (field validation, order overview, order completion) — 8 TCs
  - Logout — 1 TC
- **3 exploratory findings** using SauceDemo's special test accounts (`problem_user`, `performance_glitch_user`), which the site intentionally uses to demonstrate common UI bugs. These are documented separately in the Bug Report and are not part of the 21 formal cases.

## Results
| Module | Total TCs | Passed | Failed | Pass % |
|---|---|---|---|---|
| Login | 5 | 5 | 0 | 100% |
| Products Page | 7 | 7 | 0 | 100% |
| Checkout | 8 | 8 | 0 | 100% |
| Logout | 1 | 1 | 0 | 100% |
| **Total** | **21** | **21** | **0** | **100%** |

**Defects found:** 0 in the standard_user flow. 3 known UI issues surfaced through SauceDemo's special test accounts (image mismatch, uneditable field, artificial slowdown) — see [Bug Report](./SauceDemo_Bug_Report.xlsx).

## Tools
- Excel (manual test case documentation)

## Status
✅ Login → Checkout → Logout — 21/21 test cases executed, all passing
📝 Special test-user quirks — 3 documented as exploratory findings
