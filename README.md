# hcrs
nodejs scaffold generation for holochain-rust

This is a prototyping solution. Ideally this functionality would be built into the `hc` tool, potentially `hc scaffold` or integrated into `hc init` and `hc generate`.

Generates holochain hApp source code tree based off a single `scaffold.json` file, following these rules:

- Will not overwrite any source code in a file not prefixed with a "DO NOT MODIFY" comment
- Will generate stub files if not present
- Will generate "zome_def" from the scaffold, but functional code is placed in other modules

## Usage

- Make sure the `hc` command is in your path. (in the `holochain-rust` directory, run `make install_cmd`).
- Make sure `./holochain-rust` contains the holochain rust repo... can be a symlink

```
npm install
cd example
../bin/hcrs build
```
