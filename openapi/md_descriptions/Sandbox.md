# Sandbox testing


Credit card test – success

Please note that those credit card numbers will only work for Brazil, Colombia, Mexico, Peru and Argentina.
First, let’s try numbers of credit cards that have “infinite” funds and will always be authorized. That way, you’ll receive an approved transaction response.

You can use any of the following numbers in the test environment. Just don’t forget to read the tips below:

CVV: use any number with three digits, except American Express which CVV is four digits;
Expiration date (due date): use any period in the future.
Types
American Express
amex
378282246310005 & 378282749798722

Aura
aura
5078601870000127985

Diners Club
diners
30569309025904

Discover
discover
6011111111111117

Elo
elo
6362970000457013 & 6362971747129170

Hipercard
hipercard
6062825624254001 & 6062823936268330

Visa
visa
4111111111111111 & 4111115666052208

MasterCard
mastercard
5555555555554444 & 5555556355564617




Credit card test – decline

Please note that those credit card numbers will only work as intended for Brazil.
Now, let’s try another scenario with other numbers, that way you will receive a declined transaction response in the test environment.

They have the same rules as the other cards:

CVV: use any number with three digits, except American Express which CVV is four digits;
Expiration date (due date): use any period in the future.
Visa
visa
4716909774636285

response: insufficientFunds
Mastercard
mastercard
5102026827345142

response: invalidData
Discover
discover
6011088896715918

response: cardExpired
American Express
amex
378568775709157

response: notApproved