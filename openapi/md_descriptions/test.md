# Introduction
#### Welcome to the EBANX 3DS 2 documentation
This API definition is intended to guide you through the new 3DS 2 integration in Brazil.
### What is a Direct API
The EBANX Direct API is the transparent checkout (with no redirect) solution that allows you to accept payments by all payment methods and countries directly on your domain. Your customers will benefit from a smoother user experience as they can complete the checkout without the need to leave the store's front end.
All the requirements of the Direct API can be found in our [developers portal][9].
[9]: https://developers.ebanx.com/api-reference/ebanx-payment-api/payment-reference/reference-direct-operation/
# About 3D Secure 2
3D Secure, or 3DS, is a technical standard that adds a layer of security in online credit and debit card transactions, protecting the buyer's against unauthorised use. One of the main advantages of the protocol is the shift in liability of fraudulent chargebacks. If the transaction was authenticated, the liability of the transaction shifts from the merchant to the issuer.
Unlike the 3DS 1, the 3DS 2 simplifies the payment process by providing a larger set of cardholder information to the issuer, allowing for improved risk assessment and the ability to skip authentication challenge processes altogether for low risk transactions, leading to lower abandonment rates and better user experience.
> **Note:**
> - Currently, we offer 3DS 2 for debit card transactions in Brazil with external authentication, ie the merchant has to use his own 3DS Server.
## Payment flow
We have two major scenarios to process payments using the 3DS 2.
### 1. Merchants that have their own 3DS Server
![alt text][diagrama] 
[diagrama]: https://mrcsvg.github.io/EBANX-api-reference/assets/diagram.svg
Merchant -> External \nAuthenticator: (1) Request payment with 3DS
Note left of External \nAuthenticator: Authenticate \ncustomer
External \nAuthenticator --> Merchant: (2) Cryptogram Data
Merchant -> EBANX : (3) Payment request with Cryptogram data
EBANX --> Merchant : (4) Payment response
1. Merchant authenticates transaction using its own 3DS Server
2. Merchant gets the Cryptogram data that
3. Merchant requests a payment to EBANX using the Cryptogram data
4. EBANX process the transactions and return the result
### 2. Merchants that do not have their own 3DS Server
Under development.
# Sandbox testing
Under development.
#### Authentication without challenge and successful authorization
#### Authentication without challenge and failed authorization
#### Authentication with challenge and sucessful authorization
#### Authentication with challenge and failed authorization