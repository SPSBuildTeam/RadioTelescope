# Welcome to Radio telescope

## Commands

* `mkdocs new [dir-name]` - Create a new project.
* `mkdocs serve` - Start the live-reloading docs server.
* `mkdocs build` - Build the documentation site.
* `mkdocs -h` - Print help message and exit.

## Project layout

    mkdocs.yml    # The configuration file.
    docs/
        index.md  # The documentation homepage.
        ...       # Other markdown pages, images and other files.

Dish design:
to improve manufacturability the dish was segmented into even slices using the following considerations
angle of each slice:
/theta = 2π/N  where N = number of slices of dish
arc length of slice: 
S = 2πr/N where 2r > /lambda
focal length of dish:
f = r^2/4d where d is dish depth

Since we are trying to find the hyrogen line (1420.4 MHz) /lambda is 21.1 cm, this gives r > 10.55cm
For easy construction we set r as 15cm and N as 8, giving S = 11.78 cm
