>*Note: This repository primarily serves as a submodule for `LittleEngine` (and is bound by the same licence), but is completely standalone and free to be used in any other projects.*

### LittleEngine Asserts

*Copyright 2019 Karn Kaul*

Features:
  - Pre-assert MessageBox / X11 implementations that block the main thread and wait for user response
  - Responses include: "Assert", "Ignore ID" (turn off this assert), "Ignore All" (turn off all asserts)
  - Will break if debugger detected (MSVC / gdb)
  - Does nothing if `ASSERTS == 0` or not defined
Usage:
  - Define `ASSERTS 1` to enable
  - Include this file and call `Assert(predicate, message)`
