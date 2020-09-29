# Quick Start

Let's explore a basic usage scenario when you need to create a library for KiCad EDA consisting of an SMT 0603 capacitor. We assume you consider to solder it manually. 

1. Add the component:

    ```
    qeda add capacitor/c0603
    ```

2. Configure the library to be more convenient for manual soldering:

    ```
    qeda config pattern.density-level M
    qeda config pattern.minimum.space-for-iron 1
    ```

3. Generate the library:

    ```
    qeda generate mylib
    ```

4. Create test project for KiCad.

    Create a `sym-lib-table` file with the following contents:

    ```
    (sym_lib_table
        (lib (name mylib)(type Legacy)(uri ${KIPRJMOD}/kicadlib/mylib.lib)(options "")(descr ""))
    )
    ```

    Create a `fp-lib-table` file with the following contents:

    ```
    (fp_lib_table
        (lib (name mylib)(type KiCad)(uri ${KIPRJMOD}/kicadlib/mylib.pretty)(options "")(descr ""))
    )
    ```

   Create a `myboard.pro` file with the following contents:

    ```
    version=1
    [general]
    version=1
    [pcbnew]
    version=1
    [cvpcb]
    version=1
    [eeschema]
    version=1
    ```

5. Open the `myboard.pro` in KiCad, run Symbol Editor / Footprint Editor, and find both the schematic symbol and the PCB footprint for the C0603 capacitor.