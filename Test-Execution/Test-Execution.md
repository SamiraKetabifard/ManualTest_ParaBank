# Test Execution Report

## Execution Summary

| Metric | Count |
|---|---:|
| Total Test Cases | 16 |
| Passed | 9 |
| Failed | 7 |
| Blocked | 0 |
| Skipped | 0 |

## Pass Rate

56.25%

## Fail Rate

43.75%

## Test Execution Results

| Test Case | Category | Status |
|---|---|---|
| TC-LOGIN-001 | Smoke / Functional | PASS |
| TC-LOGIN-002 | Smoke / Functional | PASS |
| TC-FORGOT-001 | Functional | PASS |
| TC-FORGOT-002 | Negative / Validation | PASS |
| TC-REG-001 | Smoke / Functional | PASS |
| TC-REG-002 | Negative / Validation | PASS |
| TC-REG-003 | Negative / Validation | FAIL |
| TC-REG-004 | Negative / Validation | FAIL |
| TC-REG-005 | Negative / Validation | FAIL |
| TC-ACC-001 | Smoke / Functional | PASS |
| TC-ACC-002 | Functional | PASS |
| TC-ACC-003 | Functional / Boundary | PASS |
| TC-TRANSFER-001 | Functional / Business Logic | PASS |
| TC-TRANSFER-002 | Negative / Business Logic | FAIL |
| TC-TRANSFER-003 | Negative / Business Logic | FAIL |
| TC-BILL-001 | Smoke / Functional | PASS |

## Additional Executed Scenarios

The following scenarios were also explored during exploratory testing:

- Zero loan amount
- Excessive bill payment
- Profile update confirmation
- Administration functionality

These scenarios resulted in additional documented defects.

## Defect Summary

### High Severity

- BUG-004 — Same account accepted as source and destination
- BUG-005 — Transfer can result in negative account balance

### Medium Severity

- BUG-001 — Numeric City accepted
- BUG-002 — Numeric State accepted
- BUG-003 — Alphabetic Zip Code accepted
- BUG-006 — Zero loan amount causes internal error
- BUG-007 — Bill payment displays internal error

### Low Severity

- BUG-008 — Incorrect profile update confirmation message

## Overall Result

The application passed the basic smoke and positive functional scenarios tested during the session. However, several validation and business logic issues were identified during negative and boundary testing.

The most significant findings were related to fund transfer validation and account balance handling.
