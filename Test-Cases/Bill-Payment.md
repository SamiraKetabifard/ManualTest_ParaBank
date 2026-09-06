# Bill Payment Test Cases

## TC-BILL-001 — Successful Bill Payment

**Type:** Smoke / Functional / Positive

### Test Data

Amount: `$100`

### Steps

1. Open Bill Pay.
2. Enter valid payee information.
3. Enter the account information.
4. Enter `$100`.
5. Select the source account.
6. Submit the payment.

### Expected Result

The bill payment should be completed successfully and the transaction should be recorded.

### Actual Result

The bill payment was completed successfully and the transaction was displayed.

### Status

PASS

---

## TC-BILL-002 — Invalid or Excessive Bill Payment Amount

**Type:** Functional / Negative / Business Logic / Error Handling

### Steps

1. Open Bill Pay.
2. Enter valid payment information.
3. Enter an invalid or excessive payment amount.
4. Submit the payment.

### Expected Result

The system should reject the transaction and display a meaningful validation or insufficient-funds message.

### Actual Result

The system displayed:

`Error! An internal error has occurred and has been logged.`

### Status

FAIL
