# Disable-boot_out.txt-File

# It disable `boot_out.txt` file which are shown while boot the CircuitPython device.

# Steps
1. Go to `circuitpython` folder.
2. Open `main.c` file.
3. Search `bool write` in the file.
4. Change the value from `true` to `false`.
5. Save this file.
6. Done! Build, flash and `boot_out.txt` file is not shown while boot.
