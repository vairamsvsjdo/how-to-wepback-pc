# entrypoint must precede all other arguments in commandline to override
docker run --entrypoint="/bin/bassh" -it example/redis --help
