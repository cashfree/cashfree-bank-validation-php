# Cashfree Bank Validation Integration Kit for PHP

Below is an integration flow on how to use Cashfree's payouts.
Please go through the payout docs [here](https://dev.cashfree.com/payouts)
<br/>
This kit is linked to the Bank Validation flow. Go [here](https://dev.cashfree.com/payouts/integrations/bank-validation) to get a better understanding.
<br/>

## Functionalities

The following kit contains the following functionalities:
    <ol>
    <li> [getToken](https://dev.cashfree.com/api-reference/payouts-api#authorise): to get the auth token to be used in all          following calls.
    <li> [verifyBankAccount](https://dev.cashfree.com/api-reference/payouts-api#bank-verification): to verify bank account.
    </ol>

## Build Steps

follow the following build steps to compile the Integration kit:
  1. Download the code and cd into the directory containing the code.

## Set Up

### Pre Requisites:
The following kit uses information stored in the index.php file. Before running the code for the first time open the index.php file
and add the relevant details:
  1. ClientId: This is a unique identifier that identifies the merchant. For more information please go [here](https://dev.cashfree.com/development/api/credentials).
  2. ClientSecret: Corresponding secret key for the given ClientId that helps Cashfree identify the merchant. For more information please go [here](https://dev.cashfree.com/development/api/credentials).
  3. Environment: Environment to be hit. The following values are accepted prod: for production, test: for test environment.

### IP Whitelisting:

Your IP has to be whitelisted to hit Cashfree's server. For more information please go [here](https://dev.cashfree.com/development/api/ip-whitelisting).

### Bank Details:

The following kit needs bank account details to validate the bank account. For a list of required fields go [here](https://dev.cashfree.com/api-reference/payouts-api#bank-verification)
<br/>
The kit picks up the bank account details from the index.php file bankDetails object. Required fields are:
  1. name: name of the account to be verified.
  2. phone: phone number of the account holder.
  3. bankAccount: bank account to be validated.
  4. ifsc: ifsc of the corresponding bank account.


## Usage

Once the index.php file is setup you can run the executable, to run the entire flow. Authorize and validate bank account. 

run the following line in the terminal to run the script.

```
  php index.php
```

You can change the necessary values in the index.php file as per your requirements and re-run the script whenever needed.

## Doubts

Reach out to techsupport@cashfree.com in case of doubts.
 


