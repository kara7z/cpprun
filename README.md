# cpprun

Compile and run a single C++ file with one command.

## Install

**curl (single file):**
```sh
curl -sSL https://raw.githubusercontent.com/kara7z/cpprun/main/cpprun -o ~/.local/bin/cpprun && chmod +x ~/.local/bin/cpprun
```

**clone (full repo):**
```sh
git clone https://github.com/kara7z/cpprun.git && cp cpprun/cpprun ~/.local/bin/ && rm -rf cpprun
```

Make sure `~/.local/bin` is in your `PATH` (add `export PATH="$HOME/.local/bin:$PATH"` to `~/.zshrc` or `~/.bashrc` if not already).

## Usage

```sh
cpprun file.cpp [args...]
```

Compiles with `-std=c++17 -Wall -Wextra -Werror` and runs the binary, passing any additional arguments.
