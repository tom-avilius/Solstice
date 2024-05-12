
# List of Dependencies with Installation Commands


## Hyprpaper

A wallpaper utility. 
Link: [Hyprpaper](https://github.com/hyprwm/hyprpaper)

### Install its Dependencies with:
` sudo dnf install wayland-devel wayland-protocols-devel hyprlang-devel pango-devel cairo-devel file-devel libglvnd-devel libglvnd-core-devel libjpeg-turbo-devel libwebp-devel gcc-c++ `

### Install Hyprpaper with:

1. `make --no-warn-unused-cli -DCMAKE_BUILD_TYPE:STRING=Release -DCMAKE_INSTALL_PREFIX:PATH=/usr -S . -B ./build`
`cmake --build ./build --config Release --target hyprpaper -j`
\``nproc 2>/dev/null || getconf NPROCESSORS_CONF`\`
2. `cmake --install ./build`