# cpprun

Compile and run a single C++ file with one command.

## Requirements

- `g++` (install with `sudo pacman -S gcc` on Arch, `sudo apt install g++` on Debian/Ubuntu, etc.)
- `~/.local/bin` in `PATH` (add `export PATH="$HOME/.local/bin:$PATH"` to `~/.zshrc` or `~/.bashrc`)

## Install

**curl (single file):**
```sh
mkdir -p ~/.local/bin && curl -sSL https://raw.githubusercontent.com/kara7z/cpprun/main/cpprun -o ~/.local/bin/cpprun && chmod +x ~/.local/bin/cpprun
```

**clone (full repo):**
```sh
git clone https://github.com/kara7z/cpprun.git ~/.local/share/cpprun && ln -sf ~/.local/share/cpprun/cpprun ~/.local/bin/cpprun
```

## Usage

```sh
cpprun file.cpp [args...]
```

Compiles with `-std=c++17 -Wall -Wextra -Werror` and runs the binary, passing any additional arguments.
