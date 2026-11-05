# Zelda: Ocarina of Time — Lichii Windows experimental build

Source: `zortos293/Lichii` `fix/oot-fog` at `375c4a472bd95fdfaae0de6e3f192499cd14f806`.

This branch includes upstream shader lowering fixes targeting the three rejected Kokiri Forest programs (native depth comparison gather and per-tap F16 gathers), plus Vulkan frame-dump diagnostics. The code is experimental. Passing a Windows build does **not** establish that the excessive fog/bloom effect is corrected.

## Windows test checklist

1. Obtain the `windows-x86_64` artifact from GitHub Actions for this exact branch.
2. Extract to a *new* folder, leaving the existing build 75 intact.
3. Start `lichii.exe`, load the same scene and compare FPS and volumetric lighting with build 75.
4. If a problem persists, capture the native shader rejections and a frame dump with `EDEN_NX2_FRAME_DUMP` (see upstream `AGENTS.md`).

This metadata file doesn't alter emulator behavior. Gameplay corrections reside in the upstream source changes inherited by this branch.
