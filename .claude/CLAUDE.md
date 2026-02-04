# cc3dsfs - 3DS Capture Card Fullscreen Software

## Build

Rebuild from project root (in-source build):
```
cmake . && make -j$(nproc)
```

The binary is copied to the project root as `cc3dsfs` after build.

## Run

Launch with capture display settings via:
```
./run.sh
```

This runs: `./cc3dsfs --auto_connect --enabled_both 0 --enabled_top 1 --enabled_bot 1 --scaling_bot 2.8 --scaling_top 2.8`

## Project Notes

- CMake in-source build (build artifacts in project root)
- Dependencies (SFML, libusb) fetched via CMake FetchContent
- Supports multiple capture devices: Loopy, IS Nitro/TWL, Nisetro, Optimize 3DS, Partner CTR
- C++20 standard
