
# List of Dependencies with Installation Instructions (including commands)


## Hyprpaper

A wallpaper utility. 
Link: [Hyprpaper](https://github.com/hyprwm/hyprpaper)

### Do a git clone 

> I know its a basic thing but in case you forget:

Visit the [Hyprpaper](https://github.com/hyprwm/hyprpaper) page and clone the repository at a location(could be temporary).

### Install its Dependencies with:
` sudo dnf install wayland-devel wayland-protocols-devel hyprlang-devel pango-devel cairo-devel file-devel libglvnd-devel libglvnd-core-devel libjpeg-turbo-devel libwebp-devel gcc-c++ cmake`

### Install Hyprpaper with:

1. `make --no-warn-unused-cli -DCMAKE_BUILD_TYPE:STRING=Release -DCMAKE_INSTALL_PREFIX:PATH=/usr -S . -B ./build`
`cmake --build ./build --config Release --target hyprpaper -j`
\``nproc 2>/dev/null || getconf NPROCESSORS_CONF`\`
2. `sudo cmake --install ./build`

> For usage instructions see [Hyprpaper Usage](https://github.com/hyprwm/hyprpaper#usage).

__Hyprpaper setup is now complete__