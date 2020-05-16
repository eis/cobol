== Installing ==

=== Windows ===

# Get https://www.arnoldtrembley.com/GC31-GDB-B-rename-7z-to-exe.7z
# Rename to .exe
# Run the self-extracting package
# Add bin folder from the extracted directory to path
# Copy set_env.cmd from install directory to bin directory as set-cobol-env.cmd
# Change COB_MAIN_DIR line in set-cobol-env.cmd to exactly this:

```
set COB_MAIN_DIR=%~dp0..\
```

# Start cmd.exe and run
```
> set-cobol-env
```

== Compiling and running a program ==


> cobc -x hello.cob
> hello
Hello, world