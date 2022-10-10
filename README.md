# docker-compose
To allow docker to create a wordpress installation and mysql database


To download the necessary files and start the processes issue the following command;

docker-compose up

That’ll start the WordPress and database instance and show the log files on the terminal. If you want to stop the instance simply press CTRL-C and they’ll gracefully shut down.

If you want to run the Docker instances as background processes you can issue the following command instead;

docker-compose up -d

The -d flag tells Docker to ‘detach’ the process and run it in the background instead. If you look at the docker-compose.yml file that we created earlier, you’ll notice a couple of lines in there that say restart: always – these lines are used with the background task flag to tell Docker Desktop to automatically relaunch these processes if they fail or if the computer is restarted.

To stop the processes use;

docker-compose down
