pico-bme688-forced
==================

Read the BME688-sensor in _forced-mode_ on a Raspberry Pi Pico using the official API of Bosch-Sensortec.

This project is an adaption of the forced-mode example of the API.

You need to configure `CMakeLists.txt` for your needs (hardware-setup and altitude at your location).


Preparation
===========

After checkout, run

    git submodule update --init --recursive

This pulls in the [bme688-library-project](https://github.com/bablokb/pico-bme688) and the git-repo from Bosch-Sensortec.


Build
=====

Either use VSCode (preferred) or use:

    mkdir -p build
    cd build
    cmake ..
    make
    cd ..

The executable is `build/pico-bme688-forced.uf2`.
