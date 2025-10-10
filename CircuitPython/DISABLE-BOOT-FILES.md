# Disbale Boot Files

# It disables various files which are shown while boot the CircuitPython device.

# Steps to do
1. Go to `circuitpython/supervisor/shared` folder.
2. Open `filesystem.c` file.
3. Find these lines in the file.
4. Replace the line by just copy the line from given below list and paste exactly where the original line exist.
4. After done this, save the file.
5. Done! Build, flash and commented line files is not shown while boot.

# List of lines in `filesystem.c` file
```
// res = f_mkdir(&circuitpy->fatfs, "/.fseventsd");
```
```
// make_empty_file(&circuitpy->fatfs, "/.fseventsd/no_log");
```
```
// make_empty_file(&circuitpy->fatfs, "/.metadata_never_index");
```
```
// make_empty_file(&circuitpy->fatfs, "/.Trashes"); // MacOS
```
```
// make_empty_file(&circuitpy->fatfs, "/.Trash-1000"); // Linux, XDG trash spec:
```
```
// res = f_mkdir(&circuitpy->fatfs, "/sd");
```
```
// MAKE_FILE_WITH_OPTIONAL_CONTENTS(&circuitpy->fatfs, "/sd/placeholder.txt",
// "SD cards mounted at /sd will hide this file from Python.\n");
```
```
// res = f_mkdir(&circuitpy->fatfs, "/saves");
```
```
// MAKE_FILE_WITH_OPTIONAL_CONTENTS(&circuitpy->fatfs, "/saves/placeholder.txt",
// "A separate filesystem mounted at /saves will hide this file from Python."
// " Saves are visible via USB CPSAVES.\n");
```
```
// make_empty_file(&circuitpy->fatfs, "/settings.toml");
```