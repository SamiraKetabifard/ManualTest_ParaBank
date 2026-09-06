# Forgot Login Information Test Cases

## TC-FORGOT-001 — Successful Login Information Recovery

**Type:** Functional / Positive

### Steps

1. Open Forgot Login Info.
2. Enter the required user information.
3. Submit the form.

### Expected Result

The system should locate the user's login information when valid information is provided.

### Actual Result

The system displayed:

`Your login information was located successfully. You are now logged in.`

### Status

PASS

---

## TC-FORGOT-002 — Empty Required Fields

**Type:** Functional / Negative / Input Validation

### Steps

1. Open Forgot Login Info.
2. Leave required fields empty.
3. Submit the form.

### Expected Result

Validation messages should be displayed for required fields.

### Actual Result

Validation messages were displayed next to the required fields.

### Status

PASS
