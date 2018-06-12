# Tuck

Install (tuck) folder of binaries on Linux.

Nothing more than a script to prepare an application for
use on a unix environment. It copies the folder to `/opt`,
creates a sym link in `/usr/local/bin`, then finally 
sets up a file for gnome application menus in `/usr/share/applications`.

**Note:** This is a hardcoded implementation. Configurability coming soon.


## Usage

1. Clone the repo
2. Install node dependencies: `npm install`
2. Link with npm: [`npm link`](https://docs.npmjs.com/cli/link)
3. Run `tuck` in the CLI


## Requirements

[Node](https://nodejs.org/en/) version 8+
