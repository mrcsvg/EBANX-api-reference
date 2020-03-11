This is an **example** API to demonstrate features of OpenAPI specification 

# Introduction

#### Welcome to the EBANX 3DS 2.0 documentation!

This API definition is intended to guide you thru the new 3DS 2.0 integration.


### What is a Direct API

The Direct API of EBANX is the transparent checkout (with no redirect) solution that allows you to accept payments by all payment methods and countries directly on your domain.

Your customers will benefit from a smoother user experience as they can complete the checkout without the need to leave the store’s front end.

There are some requirements to follow before making the integration that you can learn here.



# About 3D Secure 2
3D Secure, or 3DS, is a technical standard that adds a layer of security in online credit and debit card transactions, protecting the buyer's against unauthorised use. One of the main advantages of the protocol is the shift in liability of fraudulent chargebacks. If the transaction was authenticated, the liability of the transaction shifts from the merchant to the issuer.

3DS 2.0 simplifies the payment process by providing a larger set of cardholder information to the issuer, allowing for improved risk assessment and the ability to skip authentication challenge processes altogether for low risk transactions, leading to lower abandonment rates and better user experience.

Currently, we offer 3DS 2.0 for debit card transactions in Brazil with external authentication.

## Payment flow

We have two major scenarios (integration-wise):
### Merchants that have their own authenticator/MPI




Reference-style: 
![alt text][diagrama] 

[diagrama]: https://mrcsvg.github.io/EBANX-api-reference/assets/diagram.svg

1. LALALA
2. LALALA2
3. LALALAL 3 


# Authentication

With just one integration, your company can sell to consumers based in Brazil, Mexico, Argentina, Colombia, Chile, Peru, and Ecuador. Offering local payment options is an excellent opportunity to increase your sales and reach even more customers.

**Request your test account**

If you don’t have your testing account yet, access our EBANX Business Page, select your business model and answer a few questions. One of our Business Development Analysts will get in touch shortly.

At this stage, you will have access to your test Integration keys. Only after the conclusion of your negotiation and the integration process with our team, you will receive your live integration keys.


# Sandbox testing

### Credit card test – success

First, let’s try numbers of credit cards that have “infinite” funds and will always be authorized. That way, you’ll receive an approved transaction response.

You can use any of the following numbers in the test environment. Just don’t forget to read the tips below:

**-CVV:** use any number with three digits, except American Express which CVV is four digits;
**-Expiration date (due date):** use any period in the future.


Brand | Cards
------ | ------
American Express    | 378282246310005 and 378282749798722
Aura                | 5078601870000127985
Diners Club         | 30569309025904
Discover            | 6011111111111117
Elo                 | 6362970000457013 and 6362971747129170
Hipercard           | 6062825624254001 and 6062823936268330
Visa                | 4111111111111111 and 4111115666052208
MasterCard          | 5555555555554444 and 5555556355564617

### Credit card test – decline

Now, let’s try another scenario with other numbers, that way you will receive a declined transaction response in the test environment.

They have the same rules as the other cards:

**-CVV:** use any number with three digits, except American Express which CVV is four digits

**-Expiration date (due date):** use any period in the future.

Brand | Cards | Response 
------ | ------ | ------
Visa | 4716909774636285 | insufficientFunds
Mastercard | 5102026827345142 | invalidData
Discover | 6011088896715918 | cardExpired
American Express | 378568775709157 | notApproved