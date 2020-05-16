## Installing

### Windows

1. Get https://www.arnoldtrembley.com/GC31-GDB-B-rename-7z-to-exe.7z
2. Rename to .exe
3. Run the self-extracting package
4. Add bin folder from the extracted directory to path
5. Copy set_env.cmd from install directory to bin directory as set-cobol-env.cmd
6. Change COB_MAIN_DIR line in set-cobol-env.cmd to exactly this:

```
set COB_MAIN_DIR=%~dp0..\
```

7. Start cmd.exe and run
```
> set-cobol-env
```

## Compiling and running a program


```
> cobc -x hello.cob
> hello
Hello, world
```
