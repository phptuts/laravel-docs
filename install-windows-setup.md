# Laravel 

1. Download and install the [Docker Desktop App](https://docs.docker.com/desktop/install/windows-install/)
2. Open a powershell and run this command to install windows for linux.  Be sure to save the password that you type in for the root password.
<img width="657" alt="image" src="https://github.com/phptuts/laravel-docs/assets/9620015/c597fcad-3b9b-446d-933e-c993c79bbd8a">

```bash
wsl --install
```

3. Restart your machine
4. Once you have restarted log back in and open a command prompt and type in wsl --version.  Be sure you are using version 2.
<img width="456" alt="image" src="https://github.com/phptuts/laravel-docs/assets/9620015/92c3c68a-0ead-4bcc-a71d-c3b25631a82a">

5. Once you have that installed open powershell again and type in wsl
6. Start up Docker Desktop App
  
8. Then run this command, the example-app will be what controls the name of the folder and app.  This command could take a few minutes to complete.  You will be asked for your password.
```bash
curl -s https://laravel.build/example-app | bash
```

8. While it working download an app called [dbeaver](https://dbeaver.io/download/).  This is how you will look at your database locally.
9. Download and Install [VS Code](https://code.visualstudio.com/)
10. Install these plugins in vs code. The plugin / extension menu is around the top left of the screen.  It's the icon with the 2 by it on the left side.
      - Auto Close Tag
      - Beautify Blade
      - Laravel Extra Intellisense
      - PHP
      - PHP Namespace Resolver
    <img width="764" alt="image" src="https://github.com/phptuts/laravel-docs/assets/9620015/0eb8ab42-670a-4d7b-90d5-a754b3c51013">

11. Run this command to start up sail to be safe
    ```bash
    vendor/bin/sail up -d
    ```
This is how you will turn on the web server

12. Next this command to create the user table for your database.
```bash
    vendor/bin/sail artisan migrate
```

13. Go to http://localhost and make sure your website is up and running.
