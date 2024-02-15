## Linux Instructions (raw)

#### SIGSEGV or Invalid Memory Reference?
```shell
export RUSTFLAGS="-Ccodegen-units=1"
```
**Reference:** [GitHub Issue](https://github.com/rust-lang/cargo/issues/6489#issuecomment-539211023)

#### Failed to locate `open-ssl` but it is installed?
```shell
sudo apt install pkg-config
```

#### Failed to locate `open-ssl` but unsure if it is installed or any of it's distros?
```shell
sudo apt install libssl-dev
```

#### Cannot find python3.10 for pyo3 to compile?
**Error:** `/usr/bin/ld: cannot find -lpython3.10`

> The error message indicates that the linker (ld) is unable to find the library libpython3.10. This typically happens when the development files for Python 3.10 are not installed.

```
sudo apt-get install libpython3.10-dev
```
