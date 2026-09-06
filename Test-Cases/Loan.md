# Loan Test Cases

## TC-LOAN-001 — Valid Loan Request

**Type:** Functional / Business Logic

### Test Data

Loan Amount: `$1500`  
Down Payment: `$100`

### Steps

1. Open Request Loan.
2. Enter `$1500` as Loan Amount.
3. Enter `$100` as Down Payment.
4. Select the required account.
5. Submit the request.

### Expected Result

The loan request should be processed according to the application's loan rules.

### Actual Result

The loan request was approved and a new loan account was created.

### Status

PASS

---

## TC-LOAN-002 — Zero Loan Amount

**Type:** Functional / Negative / Boundary / Input Validation

### Test Data

Loan Amount: `0000`

### Steps

1. Open Request Loan.
2. Enter `0000` as Loan Amount.
3. Submit the request.

### Expected Result

The system should reject a zero loan amount and display an appropriate validation message.

### Actual Result

The system displayed:

`Error! An internal error has occurred and has been logged.`

### Status

FAIL
