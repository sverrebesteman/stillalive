# *NOTE, this is not my project. This is simply a fork with pygame instead of playsound. All credit goes to https://github.com/errorer


A demo of the credit song 'Still Alive' of Portal 1 written in Python, running
in text terminal.

## Dependency

`still_alive_credit.py` is written with Python 3. In most cases the following
`pip` should be `pip3` command.

In Windows, you need a teminal emulator supporting ANSI escape sequences like Windows Terminal, MinTTY, Cmder or ConEmu.

For playing music, you need install `pygame` with `pip3`.

On macOS, you need to install python3 and pip3. What worked for me was Homebrew. 
When you have installed pip3, run `pip3 install pygame`, same as on Linux.

## Usage

In the downloaded directory, execute:

```
python3 still_alive_credit.py
```

The script will read the following environment variables: `TERM`, `COLUMNS` and `LINES` to determine
the output area size and whether to enable features such as terminal color. If you
want run it on a standard VT100 terminal, you should execute the following command:

```
TERM=vt100 python3 still_alive_credit.py
```

You can use the `--no-stay` option to automatically exit after the music finishes playing. By default, it remains on the playback screen. You can also press `Ctrl+C` to exit.

It's able to use `--no-sound` option to run the script without playing sound. In this
case, the script only depends on Python standard library:

```
python3 still_alive_credit.py --no-sound
```
