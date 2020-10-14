# Installation

> **Attention!** Only development builds for Linux, MacOS, and Windows are available at the moment.

## Installation on Linux

### Stable: From DEB Repository (Ubuntu/Debian)

Installing on Ubuntu:

```bash
curl -sL https://pkg.qeda.org/setup | sudo -E bash -
```

Installing on Debian (as root):

```bash
curl -sL https://pkg.qeda.org/setup | bash -
```

Check whether you can run QEDA from the command string:

```bash
qeda --version
```

### Development: From Package

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

## Installation on MacOS

### Stable: Using Homebrew

*Coming soon.*

<!--
1. Tap the brew:

    ```bash
    brew tap qeda/stable
    ```

2. Install:

    ```bash
    brew install qeda
    ```

3. Check whether you can run QEDA from the command string:

    ```bash
    qeda --version
    ```
-->

### Development: From Package

1. Install prerequisites if needed:

    ```bash
    brew install wget
    ```

2. Download the package with the executable binary:

    ```bash
    wget https://builds.qeda.org/dev/qeda-mac-x86_64-dev.tar.xz
    ```

3. Unpack the package and copy the `qeda` executable to `/usr/bin` directory:

    ```bash
    tar -xf qeda-mac-x86_64-dev.tar.xz
    cd qeda-mac-x86_64-dev
    sudo cp -fv qeda /usr/bin
    ```
4. Check whether you can run QEDA from the command string:

    ```bash
    qeda --version
    ```

## Installation on Windows

### Stable: Using `winget`

1. Download and install `winget` if needed:

    [https://github.com/microsoft/winget-cli/releases](https://github.com/microsoft/winget-cli/releases)

2. *Coming soon.*

<!--
2. Add the source:

    ```cmd
    winget source add --name qeda https://pkg.qeda.org/cache
    ```

3. Update and install:

    ```cmd
    winget update
    winget install qeda
    ```

4. Check whether you can run QEDA from the command string:

    ```cmd
    qeda.exe --version
    ```
-->

### Development: From Package

1. Download the package with the executable binary:

    [https://builds.qeda.org/dev/qeda-windows-x86_64-dev.7z](https://builds.qeda.org/dev/qeda-windows-x86_64-dev.7z)

2. Use [7-Zip](https://www.7-zip.org/) archive manager or similar to unpack `qeda.exe` executable from the package.

3. Copy the executable to `C:\Windows` directory or any directory that is specified in the `PATH` environment variable.

4. Check whether you can run QEDA from the command string:

    ```cmd
    qeda.exe --version
    ```
