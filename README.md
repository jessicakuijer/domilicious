## Domi'Licious - Book a chef at home!
### Projet collectif final  / soutenance - Prestations de chefs à domicile
(Copy of our collaborative project : https://github.com/BOUCHRA-ui/Domi-Licious)

![ScreenShot](https://github.com/jessicakuijer/domilicious/blob/domilicious-final/screenshot.PNG)

1. Clone this repository

2. Open and start Xampp (Apache server and MySQL)

3. Open symfony server (symfony server:start on gitbash or other terminal)

4. composer install : it will install missing dependencies for symfony

5. install database by commande lines : php bin/console doctrine:database:create & php bin/console doctrine:database:update --force

5. change .env file line APP_ENV=prod by APP_ENV=dev because you'll need it to be able to load fixtures. it won't work in production mode.

6. install fixtures by this command line if necessary : composer require doctrine/doctrine-fixtures-bundle --dev

5. php bin/console d:f:l (doctrine:fixtures:load) : it will load datas into databases, based on our different Fixtures (users, menus, type de cuisine, chefs and commentaires)

6. you can access the website on localhost:8000

7. try to log in with test6@test.com / password: pass_1234 (ROLE_USER) or admin@domilicious.com / password : admin (ROLE_ADMIN) and check the following roots:
- /admin (and access easyadmin directly or via navbar)
- /user (this page was intentionnally set as a basic array layout, to test permissions for the live demo)
- /commentaire (and write a comment into "livre d'or")
- /menu (and book a menu! you can reach pre-confirmation and paypal payment at the end)
- /contact (write a message and get results at https://mailtrap.io/signin with domicilious@gmail.com / password: domicilious1! )

Credits : made with Bouchra Trabelsi: https://github.com/BOUCHRA-ui, Mounia Jafjaf: https://github.com/Mounia-j and Almarine Grady: https://github.com/almoybf
  
