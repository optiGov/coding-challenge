# optiGov Coding Challenge

Great to have you here! You already got your instructions via the interview application.
Here are the required steps to spin up the application.

## Spin up the Laravel Sail service

***Hint:** This step requires Docker to be installed! If you are not comfortable with docker, you can edit the `.env` file and set up your own database environment.*

At first, you need to start the `laravel sail` service by executing:
```shell
./vendor/bin/sail up
```
This should spin up the docker container, containing the laravel application and a mysql database.

## Migrate database
Right after that we need to migrate the database. 
So just execute the `php artisan migrate:fresh` command. E.g. wihtin the docker container:

```shell
docker exec -ti "CONTAINER_NAME" php artisan migrate:fresh
```

## You are ready!

You are ready to go! Just follow the instructions and upload your awesome code.
We are looking forward for your submission!
