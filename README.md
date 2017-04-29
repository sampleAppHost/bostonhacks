# bostonhacks
FinTech Sample App for Authorize and Accounts

Running the skeleton application:

1. Register for an Open Banking Developer Hub Account.

2. Login to the Open Banking Developer Hub.

3. Create a new application - put 'https://127.0.0.1:3000/accounts/retrieve' as your redirect URI. Write down your client id and client secret

4. Create a new folder for your sample application.

5. Install or ensure that you have the latest versions of Node (https://nodejs.org) and OpenSSL (https://openssl.org).

6. Using OpenSSL in your new folder, execute the following command: openssl req -x509 -newkey rsa:2048 -keyout key.pem -out cert.pem -days 365
	a. write down whatever password you create
	b. for COMMON NAME, put 'localhost'
	c. verify that key.pem and cert.pem exist in your new folder

7. Place package.json, index.html, and server.js in your new folder either through direct download or git.

8. In Index.html and server.js - replace all text marked by <REPLACE WITH _______> according to the proper parameters. You will need your client ID, Secret, and certificate password. Remove the <> symbols as well.

9. in your new folder, run the following command: node server.js

10. You should get a confirmation the server is running on port 3000.

11. Navigate to https://127.0.0.1:3000 on your browser. accept the self-signed certificate, and follow the onscreen prompts to test your application. You should end on a screen that pretty prints account summaries in a JSON format.
