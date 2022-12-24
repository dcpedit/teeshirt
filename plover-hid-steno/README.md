# Small TeeShirt build and Plover

<img width="600" alt="Keymap" src="https://user-images.githubusercontent.com/800930/209450813-0da252e6-b3c7-4f91-be50-4b0cf32ebe66.png">

I've put together some documentation for those who wanted to play around with stenography.  It took some tinkering to get ZMK working with Plover, so hopefully these instructions will be helpful to those who are looking to accomplish the same thing.

## ZMK firmware

https://github.com/dcpedit/zmk-plover

This is a fork of dnaq's implementation of the Plover HID protocol in ZMK.  You can read about it in the [official pull request here.](https://github.com/zmkfirmware/zmk/pull/962)

The precompiled binary can be used as well (`zmk.uf2`)

After loading the firmware, you can test it with the following site:
https://lim.au/#/software/plover-hid

## Macs with Intel chip

Plover requires the `hidapi` package, so you will need to install it with [Homebrew](https://brew.sh/).

```
brew install hidapi
```

## Macs with ARM chip (M1, M2)

The ARM version of `hidapi` package will not work, so you will need to install the Intel (x86) version of Homebrew and hidapi  [(source)](https://gist.github.com/progrium/b286cd8c82ce0825b2eb3b0b3a0720a0).

```
$ arch -x86_64 zsh
$ /bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
```

```
$ brew install hidapi
```


## Plover software

Now download and install the Plover software: https://www.openstenoproject.org/plover/


## Plover HID Plugin

Download or clone https://github.com/dnaq/plover-machine-hid

Then switch to the directory where the plugin files are located.

```
cd plover-machine-hid
```

Follwing the [Plover instructions for installing plugins](https://plover.readthedocs.io/en/latest/plugins.html), run the command below (examples are for a Mac)

```
/Applications/Plover.app/Contents/MacOS/Plover -s plover_plugins install -e .
```

To list installed plugins

```
/Applications/Plover.app/Contents/MacOS/Plover -s plover_plugins list
```

## Configure Plover

Start the Plover application, click the **Configure** button, and then go to the **Machine** tab.  Select `Plover HID` in the **Machine** dropdown.

Double click on each of the **Action** cells in the right column and select the action that matches the left column.  Then click the **OK** button to go back to the main screen.

<img width="583" alt="Configure" src="https://user-images.githubusercontent.com/800930/209448146-f590aa77-fe76-4a90-a4fc-9112d343f506.png">

Select the `Plover HID` Machine and then click select `Enable`.

<img width="441" alt="Plover-HID" src="https://user-images.githubusercontent.com/800930/209448150-a9210cb2-3003-4c78-ab9d-b560efa78b5e.png">

## Start typing!

And that's it!  The middle button on the TeeShirt will toggle the Plover layer on and off.  Here's a good resource if you're just starting out with Plover:

https://sites.google.com/site/learnplover/home
