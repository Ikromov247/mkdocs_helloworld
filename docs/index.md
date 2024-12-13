# Welcome to Docker Basics tutorial

This documentation will serve as reference for working with Docker.
Full official documentation is available at <a href="https://docs.docker.com/" target="_blank" title="Docker Docs in a new page">🐳Docker docs</a> 

## Basic Commands

* `docker build Dockerfile` - Build a new docker image from a Dockerfile in the current directory.
* `docker start image_name` - Start a new container from an image.
* `docker ps` - Check running containers.
* `docker images` - Check images.

## Project layout

    Dockerfile    # The Dockerfile for building the images.
    code/
        main.py  # The code that will be run inside docker container.

```py title="add_two_numbers.py" linenums="1" hl_lines="2-4"
# Function to add two numbers
def add_two_numbers(num1, num2):
    return num1 + num2

# Example usage
result = add_two_numbers(5, 3)
print('The sum is:', result)
```

??? warning "Important to remember"

    Sometimes you may need to sleep at night.