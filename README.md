# Position-Based-Dynamics
Position Based Dynamics with Simple Visualization

Requirements
============
Support platforms: Windows, Linux 

## Dependencies

| Name                                   | Version | Usage                                               | Import         |
| -------------------------------------- | ------- | --------------------------------------------------- | -------------- |
| eigen3                                 | 3.4.0   | matrix calculation                                  | package        |
| freeglut                               | 3.4.0   | visualization                                       | package        |
| glew                                   | 2.2.0#3 | visualization                                       | package        |

### linux

We use CMake to build the project.

```bash
sudo apt install libglew-dev freeglut3-dev libeigen3-dev
```


### Windows
We use [vcpkg](https://github.com/microsoft/vcpkg) to manage the libraries we need and use CMake to build the project. The simplest way to let CMake detect vcpkg is to set the system environment variable `CMAKE_TOOLCHAIN_FILE` to `(YOUR_VCPKG_PARENT_FOLDER)/vcpkg/scripts/buildsystems/vcpkg.cmake`

```shell
vcpkg install eigen3 freeglut glew
```