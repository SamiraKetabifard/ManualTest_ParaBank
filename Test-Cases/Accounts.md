# Account Test Cases

## TC-ACC-001 — View Account Overview

**Type:** Smoke / Functional

### Steps

1. Login to ParaBank.
2. Open Accounts Overview.

### Expected Result

The system should display account numbers, balances, available balances, and total balance.

### Actual Result

Account information was displayed.

### Status

PASS

---

## TC-ACC-002 — View Account Details

**Type:** Functional

### Steps

1. Open Accounts Overview.
2. Select an account.

### Expected Result

The system should display account number, account type, balance, available balance, and transaction options.

### Actual Result

Account details and transaction options were displayed.

### Status

PASS

---

## TC-ACC-003 — Open New Savings Account

**Type:** Functional / Boundary

### Test Data

Initial Deposit: `$100`

### Steps

1. Open Open New Account.
2. Select Savings.
3. Select an existing account.
4. Use the minimum required deposit.
5. Click Create.

### Expected Result

The new savings account should be created successfully.

### Actual Result

The account was successfully created.

### Status

PASS
