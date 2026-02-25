# *NOTE, this is not my project. This is simply a fork with the sound fixed. All credit goes to https://github.com/errorer


A demo of the credit song 'Still Alive' of Portal 1 written in Python, running
in text terminal.

## Dependency

`still_alive_credit.py` is written with Python 3. In most cases the following
`pip` should be `pip3` command.

In Windows system, you need a teminal emulator supporting ANSI escape sequences
like Windows Terminal, MinTTY, Cmder or ConEmu。

For playing music, you need install `playsound` with `pip`. In Linux `playsound`
depends on `python-gobject` (default installed in Ubuntu). In MacOS you also need
to use `pip` to install `PyObjC`.

## Usage

In current directory, execute:

```
python3 still_alive_credit.py
```

The script will read environment variable `TERM`, `COLUMNS` and `LINES` to determine
the output area size and whether to enable features such as terminal color. If you
want run it on a standard VT100 terminal, you should execute:

```
TERM=vt100 python3 still_alive_credit.py
```

You can use the `--no-stay` option to automatically exit after the music finishes playing. By default, it remains on the playback screen. You can also press `Ctrl+C` to exit.

It's able to use `--no-sound` option to run the script without playing sound. In this
case, the script only depends on Python standard library:

```
python3 still_alive_credit.py --no-sound
```
