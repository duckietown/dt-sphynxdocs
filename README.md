# Duckietown ROS API docs

This container builds and combines the API docs for several Duckietown containers.

## How to use
To generate the documentation you need to build the container and run it. This is conveniently packed in the following command. Note that the mounted `output` folder is where the resulting `html` files will be copied to.
```
docker run --rm -v "$(pwd)/output":/output $(docker build -q .)
```

## Adding a new repository
To add a new repository, edit the `repositories.txt` and `docs/source/repositories.rst` files. 