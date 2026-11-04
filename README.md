# twinfetch

[fastfetch](https://github.com/fastfetch-cli/fastfetch) with a spinning ASCII Aphex Twin logo.

## Requirements

- Python 3
- fastfetch
- Linux or macOS

## Install

```sh
install -m 755 twinfetch ~/.local/bin/twinfetch
```

## Usage

```
twinfetch [-s SECONDS] [-- fastfetch args...]
```

The logo spins until a key is pressed or Ctrl-C. With `-s SECONDS`, it spins for that long, then finishes the current turn and settles facing front.

Arguments after `--` are passed to fastfetch. If output isn't a terminal, or the terminal is too short to fit the animation, twinfetch prints a single static frame.
