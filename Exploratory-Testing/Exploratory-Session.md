# Exploratory Testing Session

## Application

ParaBank

## Testing Type

Exploratory Manual Testing

## Objective

Explore the ParaBank application, identify its main features, test different user flows, and identify potential defects.

## Areas Explored

### Registration

Tested:

- Valid registration
- Password confirmation
- Numeric input in City
- Numeric input in State
- Alphabetic input in Zip Code

Observations:

- Password mismatch validation worked correctly.
- City accepted numeric input.
- State accepted numeric input.
- Zip Code accepted alphabetic input.

### Login

Tested:

- User login
- Logout
- Login after logout

### Forgot Login Information

Tested:

- Valid account information
- Empty required fields
- Successful login information recovery

Observation:

The feature successfully located the login information when valid information was provided.

### Account Management

Tested:

- Accounts Overview
- Account Details
- Account balances
- Transaction information
- Open New Account

### Transfer Funds

Tested:

- Transfers between accounts
- Transfer to the same account
- Transfer amount greater than available balance

Observations:

- Same source and destination account was accepted.
- A transfer could result in a negative source account balance.

### Bill Payment

Tested:

- Successful bill payment
- Invalid/excessive payment amount

Observation:

An internal error was displayed for one invalid/excessive payment scenario.

### Loan Request

Tested:

- Valid loan request
- Large loan request
- Zero loan amount

Observation:

A zero loan amount resulted in an internal error instead of a validation message.

### Update Contact Information

Tested:

- Updating user information
- Confirmation message

Observation:

The confirmation message did not accurately describe the information that was changed.

### Administration

Explored:

- JMS Service
- Data Access Modes
- SOAP
- REST XML
- REST JSON
- JDBC
- WSDL
- WADL
- OpenAPI
- Application Settings
