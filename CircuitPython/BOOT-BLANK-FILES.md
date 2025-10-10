# Boot-Blank-Files

# It creates blank files and folders which are shown while boot the CircuitPython device.

# Steps
1. Go to `circuitpython/supervisor/shared` folder.
2. Open `filesystem.c` file.
3. Search these lines in the file.
```
MAKE_FILE_WITH_OPTIONAL_CONTENTS(&circuitpy->fatfs, "/code.py", "print(\"Hello World!\")\n");
```
```
res = f_mkdir(&circuitpy->fatfs, "/lib");
```
4. Remove `print(\"Hello World!\")\n` and keep it blank to create a blank `code.py` file.
5. If want to create other blank file, then just copy the `code.py` line and paste under that line and change the file name from `code.py` to `YourName.py`.
6. If frozen modules are added, then disable the `/lib` folder line by adding `//` before the line.
7. If want to create other blank folder, then just copy the `/lib` line and paste under that line and change the folder name from `/lib` to `/YourName`.
8. Save the file.
9. Done! Build, flash and your custom files are shown while boot.