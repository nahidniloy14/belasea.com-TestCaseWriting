# Belasea E-Commerce: Manual Test Cases & Bug Reports

Manual QA project testing the **Register Account** feature of [Belasea](https://belasea.com), an e-commerce website and mobile app. Prepared as part of my QA training at IT Training BD (December 2022).

## Summary

| Platform | Test cases | Passed | Failed | Bugs logged |
|---|---|---|---|---|
| Website | 27 | 20 | 7 | 6 |
| Mobile app (Android) | 5 | 5 | 0 | 0 |
| **Total** | **32** | **25** | **7** | **6** |

## Scope

**Website registration**
- Registering with valid, invalid, and existing account details
- Mandatory field warnings, placeholders, and required-field markers
- Email, phone number, and password validation (mismatch, spaces, trimming)
- Email/OTP confirmation after registration
- Keyboard-only navigation (Tab, Space, Enter)
- Privacy Policy / Terms checkbox and links
- UI checks: breadcrumb, page heading, URL, title, spelling, colors, and element sizes
- Data storage and behavior across supported environments

**Mobile app registration**
- Phone number format validation
- OTP delivery and verification
- Logo display and spelling in the UI

## Key bugs found

| Bug ID | Issue |
|---|---|
| RegisterBug_001 | Submitting a fully completed registration form returned a **500 server error** |
| RegisterBug_002 | No confirmation email or OTP was sent after registration |
| RegisterBug_003 | The phone number field accepted invalid numbers |
| RegisterBug_004 | No country code option for the phone number field |
| RegisterBug_005 | Mandatory fields were not marked with a red `*` |
| RegisterBug_006 | Keyboard-only registration failed, and the phone field accepted spaces |

Screenshots are in [`Bug Screenshots/`](Bug%20Screenshots).

## Test case format

Each test case in the spreadsheets includes:

`Test Case ID` · `Test Scenario` · `Module` · `Feature` · `Type of Testing` · `Pre-requisites` · `Test Data` · `Test Steps` · `Expected Result` · `Actual Result` · `Pass/Fail` · `Bug ID` · `Screenshot` · `Comments`

Test cases were written from the project's FRS (Functional Requirement Specification) document.

## Repository structure

```
TestCases/
├── Belasea Website.xlsx            # 27 website test cases + scenario summary
└── Belasea Mobile Application.xlsx # 5 mobile app test cases
Bug Screenshots/                    # Evidence for logged bugs
```

## Tools

Microsoft Excel · Chrome browser · Android device

## Author

**Nahid Hassan Niloy**  
[LinkedIn](https://www.linkedin.com/in/nahidniloy14) · [GitHub](https://github.com/nahidniloy14)
