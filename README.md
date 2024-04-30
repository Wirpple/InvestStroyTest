# Custom Form Localization

Configure the locale environment variable in `.env` to change the form's language settings.

```env
###> symfony/framework-bundle ###
# ...other configurations...
APP_SECRET=YOUR_APP_SECRET
APP_LOCALE=ru # Available options: ru, en, ru2
###< symfony/framework-bundle ###
```

Use the following commands to start and stop the Symfony server:
To start the server:
```bash
    symfony server:start
```

To stop the server:
```bash
    symfony server:stop
```

Access the Form
Navigate to the form using the URL: ```https://localhost/form```

Done) 
