# Blommy Craft
A minecraft clone, made with modern GLFW, Modern OpenGL, CMake and VCPKG.

## Getting Started
Clone the repo with the `--recurse-submodules` flag
```bash
git clone --recurse-submodules https://github.com/JacobRBlomquist/Blommy_Craft.git
```

Run `./vcpkg/bootstrap-vcpkg.sh` or `.\vcpkg\bootstrap-vcpkg.bat`

Fetch the dependencies (see [vcpkg.json](vcpkg.json)) 
(_This is optional, CMake should run `vcpkg install` automatically_)
```bash
./vcpkg/vcpkg install
```

Build the project using your IDE/build tool of choice, or manually:

```bash
mkdir build
cmake -B build -S .
cmake --build build
```

## Troubleshooting

If you run into any problems, ensure that CMake can see the toolchain file located: `vcpkg/scripts/buildsystems/vcpkg.cmake`.

Try clearing the CMake cache or completely deleting the build folder.

