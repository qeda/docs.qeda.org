# QEDA Documentation

[![Publish Status](https://github.com/qeda/docs.qeda.org/workflows/Publish/badge.svg)](https://github.com/qeda/docs.qeda.org/actions)

Documentation for QEDA project.

:point_right: https://docs.qeda.org

## Contribution

0. Install Rust language using [rustup](https://rustup.rs/).

1. Install [mdBook](https://github.com/rust-lang/mdBook):

    ```bash
    cargo install mdbook --vers "0.4.3"
    # or
    make prepare
    ```

2. Edit source files then save.

3. Build documentation:

    ```bash
    mdbook build
    # or
    make
    ```

4. View:

    ```bash
    mdbook serve
    # or
    make serve
    ```

    Then open in browser: http://localhost:3000/

5. Create a pull-request.

## License

This repository is licensed under the [MIT license](LICENSE).
