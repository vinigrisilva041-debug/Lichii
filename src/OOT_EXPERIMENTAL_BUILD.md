# Zelda: Ocarina of Time — Lichii experimental branch

This branch is based on upstream `zortos293/Lichii` branch `fix/oot-fog` at commit `375c4a472bd95fdfaae0de6e3f192499cd14f806`.

The branch contains experimental native shader lowering changes targeting the three rejected programs identified during Kokiri Forest rendering, as well as additional Vulkan frame-capture diagnostics. These changes were developed upstream; they have **not** been verified to correct all bloom/fog effects on Windows.

This file marks the Windows build test. It does not alter emulator behavior. The actual fixes are in the source files inherited from the upstream branch.
