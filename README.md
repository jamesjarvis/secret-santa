# Secret Santa

The secret santa this year will be based on the [Pimoroni Badger 2040](https://shop.pimoroni.com/products/badger-2040?variant=39752959852627).
The goal is to create a new application that can display an interesting quote.
Still not sure if this will be fun or not, but meh sounds kinda cool.

## Step 1: Retrieve quotes

The quotes will be found from goodreads.

This will be contained under scraper/
in order to run this, run the following in that directory.

```bash
poetry install

poetry run python3 scraper.py
```

## Step 2: Quotes application

Useful command whilst developing to connect to board:

```bash
rshell -p /dev/tty.usbmodem101  --buffer-size 512
```

I've just developed this within a fork of the pimoroni-pico repository.
https://github.com/jamesjarvis/pimoroni-pico
TBH, I didn't want to bother working out how to build things from scratch on
my machine, so I just copied their github actions for building UF2 bundles.
