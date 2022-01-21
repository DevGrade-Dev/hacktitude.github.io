[<< home](./README.md)

# Challenge 16

Personally Identifiable Information (PII) should be handled carefully inside a software product. There are several personal data regulatory requirements such as GDPR you will need to adhere.

## Challenge 16.a [6 Points]

Although passwords are hashed in the database currently, the email address is stored as plain text.

As a privacy control, you are required to encrypt the email address as well in the database. The email of the user should be encrypted and saved at the time of user sign up.

The cryptographic library to use - `https://www.npmjs.com/package/crypto-js`
Encryption Key to be used - `Hacktitude_SECRET_KEY`
Encryption algorithm to use -  `AES`

Once the email is encrypted and saved in the database, you are required to update the sign-in workflow to factor in the encrypted emails.

In `seed data`, the emails of the users are stored without encryption. *Therefore please note that your new sign-in implementation must be backward compatible.* That means, the sign in workflow should work with previously stored non encrypted emails as well as new encrypted emails.

>Note: If you do not make this implementation backward compatible **ALL** the tests in the solution will fail. This is because, every test in the test suite uses the sign-in workflow to create an authenticated session for the test to run.
