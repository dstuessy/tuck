# Tuck

Install (tuck) folder of binaries in your GNOME environment.

Nothing more than a script to prepare an application for
use on a GNOME environment. It copies the folder to `/opt`,
creates a sym link in `/usr/local/bin`, then finally 
sets up a file for GNOME application menus in `/usr/share/applications`.

**Note:** This is a hardcoded implementation. Configurability coming ~~soon~~whenever anyone feels like it :shrug:.


## Usage

1. Clone the repo
2. Install node dependencies: `npm install`
2. Link with npm: [`npm link`](https://docs.npmjs.com/cli/link)
3. Run `tuck` in the CLI


## Requirements

Node version 8+


## Running with sudo

Here's a neat set of commands that will let you run `tuck` in sudo.

```
n=$(which node); \
n=${n%/bin/node}; \
chmod -R 755 $n/bin/*; \
sudo cp -r $n/{bin,lib,share} /usr/local
```

source: [stack overflow][1]


[1]: https://stackoverflow.com/questions/21215059/cant-use-nvm-from-root-or-sudo

