# Transfer Funds Test Cases

## TC-TRANSFER-001 — Transfer Funds Between Accounts

**Type:** Smoke / Functional / Business Logic

### Steps

1. Open Transfer Funds.
2. Enter a valid transfer amount.
3. Select the source account.
4. Select a different destination account.
5. Submit the transfer.

### Expected Result

The specified amount should be deducted from the source account and credited to the destination account.

### Actual Result

The transfer was completed.

### Status

PASS

---

## TC-TRANSFER-002 — Transfer to the Same Account

**Type:** Functional / Negative / Business Logic

### Test Data

Amount: `$1500`  
From Account: `13788`  
To Account: `13788`

### Steps

1. Open Transfer Funds.
2. Enter `$1500`.
3. Select account `13788` as the source account.
4. Select account `13788` as the destination account.
5. Submit the transfer.

### Expected Result

The system should reject a transfer when the source and destination accounts are identical.

### Actual Result

The system displayed:

`Transfer Complete!`

`$1500.00 has been transferred from account #13788 to account #13788.`

### Status

FAIL

---

## TC-TRANSFER-003 — Transfer Greater Than Available Balance

**Type:** Functional / Negative / Boundary / Business Logic

### Steps

1. Open Transfer Funds.
2. Enter an amount greater than the available balance.
3. Select the source account.
4. Select a different destination account.
5. Submit the transfer.
6. Open Accounts Overview.

### Expected Result

The system should reject the transfer when sufficient funds are not available, unless overdraft functionality is explicitly supported.

### Actual Result

The transfer was accepted and the source account could become negative.

### Status

FAIL
