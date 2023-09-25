# RAD Dependencies

This repository contains archives for each supported platform with the following
dependencies for building RAD:

| **Name** | **Version** |
|----------|-------------|
| ONNXRuntime | 1.16.0 |
| OpenCV | 4.8.0 |
| OneTBB | 2021.10.0 |

The goal is to facilitate the building of RAD by providing the pre-built dependencies with
the necessary flags.

## Usage

If you're building RAD from source, then do the following:

```sh
git clone https://github.com/marovira/rad.git
cd rad
git clone https://github.com/marovira/rad_deps.git _deps
cmake --preset=<preset-name> -DCMAKE_PREFIX_PATH=./_deps
cd ./build
cmake --build .
```

If you're building a project that depends on RAD, do the same steps as before, changing
the commands to clone RAD with the necessary steps for your project.

## License

This repository is published under the BSD-3 license and can be viewed [here](LICENSE).
Bundled libraries are distributed with their corresponding licenses which can be viewed
[here](LICENSE-3RD-PARTY).
