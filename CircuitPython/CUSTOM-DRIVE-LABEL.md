# Custom-Drive-Label

# It changes the drive name of the CircuitPython device when it connected to the system.

# There are `2` ways to change drive label : 

## Way - 1
1. Go to `ports/board_name_folder` folder.
2. Then, go to `boards` folder.
3. Choose your board folder.
4. Go inside the folder.
5. Open `mpconfigboard.h` file.
6. Add this line :
```
#define CIRCUITPY_DRIVE_LABEL "YOURNAME"
```
7. Replace `YOURNAME` with name what you want.
8. Save this file.
9. Done! Build, flash and drive name is show what you set.

## Way - 2
1. Go to `circuitpython/supervisor/shared` folder.
2. Open `filesystem.c` file.
3. Find this line :
```
res = f_setlabel(&circuitpy->fatfs, "CIRCUITPY");
```
4. Replace `CIRCUITPY` with name what you want.
5. Save this file.
6. Done! Build, flash and drive name is show what you set.

## Note
1. The lenght of name is only `11` characters.
2. It contain only `UPPERCASE`, `SPACE`, `UNDERSCORE` and `NUMBERS`.