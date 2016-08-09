# steamrun
A simple script for executing programs in the Steam Runtime

## Usage
```
steamrun [OPTIONS...] [PROGRAM [OPTIONS...]]

-h      Show this help
-d      Disable library workarounds
-v      Display version information
```

### Library Workarounds
The following system libraries are preloaded by the script by default, due to [known incompatibilities](https://wiki.archlinux.org/index.php/Steam/Troubleshooting#Steam_runtime_issues) of the Steam Runtime:
```
libstdc++.so.6
libgcc_s.so.1
libxcb.so.1
libgpg-error.so
```
This behavior can be disabled using the `-d` command-line option.
