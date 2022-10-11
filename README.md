
Quicl note on test :
The line in welcome.blade.php :

@php
    $user = Users::first(1);
@endphp

I could have just commented this out to get the welcome page to show, however it seemed like you wanted to be able to display data from the users table on this page at some point in the future, so I migrated and seeded the user table and made a UserController class, which is where the aove line should be, then passed the $user object to the page, to demonstrate how this should be done


Instructions for installation :

  git clone https://github.com/alexwindsor/halotest1.git

  make a mysql database called halotest1

  edit .env file with your login credentials

  php artisan migrate --seed
