# Registration Test Cases

## TC-REG-001 — Successful User Registration

**Type:** Smoke / Functional / Positive

### Steps

1. Open the Registration page.
2. Enter valid First Name.
3. Enter valid Last Name.
4. Enter valid Address.
5. Enter valid City.
6. Enter valid State.
7. Enter valid Zip Code.
8. Enter valid Phone Number.
9. Enter valid SSN.
10. Enter a valid Username.
11. Enter a valid Password.
12. Enter the same value in Confirm Password.
13. Click Register.

### Expected Result

The user should be successfully registered.

### Actual Result

The user was successfully registered.

### Status

PASS

---

## TC-REG-002 — Password Confirmation Validation

**Type:** Functional / Negative / Input Validation

### Steps

1. Open the Registration page.
2. Enter valid registration information.
3. Enter different values in Password and Confirm Password.
4. Click Register.

### Expected Result

The registration should be rejected and a validation message should be displayed.

### Actual Result

A validation message was displayed indicating that the passwords must match.

### Status

PASS

---

## TC-REG-003 — Numeric Value in City Field

**Type:** Functional / Negative / Input Validation

### Test Data

City: `455`

### Steps

1. Open the Registration page.
2. Enter `455` in the City field.
3. Complete the remaining required fields.
4. Submit the registration form.

### Expected Result

The City field should reject numeric-only input.

### Actual Result

The City field accepted `455`.

### Status

FAIL

---

## TC-REG-004 — Numeric Value in State Field

**Type:** Functional / Negative / Input Validation

### Test Data

State: `425`

### Steps

1. Open the Registration page.
2. Enter `425` in the State field.
3. Complete the remaining required fields.
4. Submit the registration form.

### Expected Result

The State field should reject numeric-only input.

### Actual Result

The State field accepted `425`.

### Status

FAIL

---

## TC-REG-005 — Alphabetic Value in Zip Code

**Type:** Functional / Negative / Input Validation

### Test Data

Zip Code: `jjgk`

### Steps

1. Open the Registration page.
2. Enter `jjgk` in the Zip Code field.
3. Complete the remaining required fields.
4. Submit the registration form.

### Expected Result

The Zip Code field should reject alphabetic input.

### Actual Result

The Zip Code field accepted `jjgk`.

### Status

FAIL
