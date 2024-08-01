# clustal-omega-apple-silicon

## Installation
1. Ensure Xcode tools are installed (`xcode-select –-install`).
2. Install Homebrew (https://brew.sh).
3. Install argtable by running `brew install argtable`.
4. Apple's version of clang included in the Xcode tools has OpenMP support disabled. If OpenMP support is desired, install conda (https://docs.conda.io/en/latest/). Then install the compilers Conda package from conda-forge `conda install conda-forge::compilers`. I recommend installing the compilers in their own Conda environment. Do this by creating a new environment with `conda create -n [myenv]` and activating it with `conda activate [myenv]` before running the install command.
5. Then run the following commands:
```
./configure CFLAGS='-I/opt/homebrew/include' LDFLAGS='-L/opt/homebrew/lib'
make
make install
```

