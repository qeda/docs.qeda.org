# Quick Installation

> **Attention!** Only development builds for Linux and Windows are available at the moment.

## Installation on Linux

1. Download the package with the executable binary:

    ```bash
    wget https://builds.qeda.org/dev/qeda-linux-x86_64-dev.tar.xz
    ```

2. Unpack the package and copy the `qeda` executable to `/usr/bin` directory:

    ```bash
    tar -xf qeda-linux-x86_64-dev.tar.xz
    cd qeda-linux-x86_64-dev
    sudo cp -fv qeda /usr/bin
    ```
3. Check whether you can run QEDA from the command string:

    ```bash
    qeda --version
    ```

    You should see something like:

    ```bash
    qeda 0.0.4
    ```

## Installation on Windows

1. Download the package with the executable binary:

    [https://builds.qeda.org/dev/qeda-windows-x86_64-dev.7z](https://builds.qeda.org/dev/qeda-windows-x86_64-dev.7z)

2. Use [7-Zip](https://www.7-zip.org/) archive manager or similar to unpack `qeda.exe` executable from the package.

3. Copy the executable to `C:\Windows` directory or any directory that is specified in the `PATH` environment variable.

4. Check whether you can run QEDA from the command string:

    ```cmd
    qeda.exe --version
    ```

    You should see something like:

    ```cmd
    qeda 0.0.4
    ```
