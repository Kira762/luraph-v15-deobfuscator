# Luau Deobfuscator

A Python tool for tracing and devirtualizing protected Roblox Luau scripts. The supplied project includes Luraph v15 and IronBrew1 support, research notes, and small regression samples.

## Usage

```sh
python3 deobf/deob.py --help
python3 deobf/deob.py path/to/input.lua
```

The tool needs Luau and `luau-ast` executables. The source archive does not include those binaries; see `deobf/build_luau.py` and the project notes (`LURAPH.md`, `IRONBREW1.md`, and `CLAUDE.md`) for implementation details and runtime requirements. The default output is written under the input file's `output/` folder.

## Contents

- `deobf/` — deobfuscator, runtime harness, and obfuscator plugins
- `samples/` — bundled regression inputs and reference outputs
- `LURAPH.md`, `IRONBREW1.md`, `CLAUDE.md` — technical notes

No license file was included in the supplied archive.
