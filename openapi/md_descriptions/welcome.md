# Introduction
#### Welcome to the EBANX 🦄 API documentation
This API definition is intended to guide you through our integrations.
### EBANX Direct API
The EBANX Direct API is the transparent checkout (with no redirect) solution that allows you to accept payments by all payment methods and countries directly on your domain. Your customers will benefit from a smoother user experience as they can complete the checkout without the need to leave the store's front end.
All the requirements of the Direct API can be found in our [developers portal](https://developers.ebanx.com/api-reference/ebanx-payment-api/payment-reference/reference-direct-operation/)


# Documentation Changelog

This is just a change log to guide us until the final launch of this documentation... After that, it is going to be replaced by our API Changelog.

## Changelog 👀

### v0.2

First big version with basic API reference for:
- Before payment
    - FX, Tokenization
- Make a payment
    - Credit card payment to all the countries
    - Payment page 
- After payment
    - Cancel and refund 
- Utils
    - Document balance, ZipCode, Tracking, Query, Print, BankList

## Comming soon 💪
### v0.3
- Payout documentation

### v0.4
- Texts review;
- Deployment to EBANX domain on github pages;
- Feedback channel;

### v0.5
- Better user of markups
- 3DS Documentation again 😅
- AMOPs (Focused in Cash payment)



# Authentication
With just one integration, your company can sell to consumers based in Brazil, Mexico, Argentina, Colombia, Chile, Peru, and Ecuador. Offering local payment options is an excellent opportunity to increase your sales and reach even more customers.   


### Request your test account
If you don't have your testing account yet, access our **EBANX Business Page**, select your business model and answer a few questions. One of our Business Development Analysts will get in touch shortly. At this stage, you will have access to your test Integration keys. Only after the conclusion of your negotiation and the integration process with our team, you will receive your live integration keys.  


# Sandbox testing  

Below you can find test card numbers and other information to make sure your integration is working as planned 😎! 
You any of the following test card numbers, a valid expiration date in the future, and any random CVC number, to create a successful payment.

- **CVV:** Use any number with three digits, except American Express which CVV is four digits;  
- **Expiration date (due date):** Use any period in the future.  

### Basic credit card numbers for testing

Brand | Cards
------ | ------
American Express    | `378282246310005` or `378282749798722`  
Aura                | `5078601870000127985`
Diners Club         | `30569309025904`
Discover            | `6011111111111117`
Elo                 | `6362970000457013` or `6362971747129170`
Hipercard           | `6062825624254001` or `6062823936268330`
Visa                | `4111111111111111` or `4111115666052208`
MasterCard          | `5555555555554444` or `5555556355564617`


### Credit card numberds for specific responses and errors

The following test cards can be used to create payments that produce specific responses—useful for testing different scenarios and error codes.

Brand | Cards | Response 
------ | ------ | ------
Visa | `4716909774636285` | insufficientFunds
Mastercard | `5102026827345142` | invalidData
Discover | `6011088896715918` | cardExpired
American Express | `378568775709157` | notApproved
