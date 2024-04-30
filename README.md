# Custom Form Localization

Configure the locale environment variable in `.env` to change the form's language settings.

```env
###> symfony/framework-bundle ###
# ...other configurations...
APP_SECRET=YOUR_APP_SECRET
APP_LOCALE=ru # Available options: ru, en, ru2
###< symfony/framework-bundle ###
```
**Running the Application**

Use the following commands to start and stop the Symfony server:

To start the server:
```bash
    symfony server:start
```

To stop the server:
```bash
    symfony server:stop
```

**Access the Form**

Navigate to the form using the URL: ```https://localhost/form```

**Screenshot**

Here is what the form looks like:
<img width="1440" alt="Снимок экрана 2024-04-30 в 12 18 31 PM" src="https://github.com/Wirpple/InvestStroyTest/assets/121581272/38cd11ea-8149-401a-9e2e-78e433facb29">

Done) 

***General information***

The ```YOUR_APP_SECRET``` in Symfony applications is a unique and secret string that is used by the application for encrypting cookies, generating CSRF tokens, and for other security-related tasks. Here are the steps for generating a new APP_SECRET:

1. Open a terminal or command prompt.

2. You can use the openssl command to generate a secret. Type the following command and press Enter:

```openssl rand -hex 32```

This will generate a 64-character hexadecimal string, which is suitable for use as an ```APP_SECRET```.

3. Copy the generated string.

4. Open your ```.env``` file in your Symfony project.

5. Find the line containing ```APP_SECRET=``` and replace the existing secret with the new one you just copied.
It would look something like this:

Replace 32characterHexStringGeneratedAbove with the actual string that openssl provided.
Remember to keep your ```APP_SECRET``` private and not to expose it in public repositories or where it can be accessed by unintended parties, as it is integral to the security of your application.
