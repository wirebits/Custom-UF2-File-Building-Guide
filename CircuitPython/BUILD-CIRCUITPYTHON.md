# CircuitPython-Custom-UF2-Build

# Steps to build custom circuitpython `.uf2` files
1. Update and Upgrade the Linux System
```
sudo apt update && sudo apt full-upgrade -y
```
2. Install Tools
```
sudo apt install git build-essential cmake gcc-arm-none-eabi libnewlib-arm-none-eabi -y
```
3. Download Circuitpython
```
git clone https://github.com/adafruit/circuitpython
```
4. Go to `circuitpython` folder
```
cd circuitpython
```
5. Install and upgrade essential python packages
```
pip3 install --upgrade -r requirements-dev.txt -r requirements-doc.txt --break-system-packages
```
6. Update Submodules
```
git submodule update --init --recursive
```
- Wait for sometime to complete.
7. Build `mpy-cross`
```
make -C mpy-cross
```
- Wait for sometime to complete.
8. Open Terminal in the folder.
9. Build `.uf2` file for your board by execute the following command : 
```
make -C ports/folder_name BOARD=folder_name_of_that_board -j$(nproc)
```
- Wait for sometime to complete.
10. Go to `build-folder_name_of_that_board`
```
cd ports/folder_name/build-folder_name_of_that_board
```
11. There is a file named `firmware.uf2` and this is your `.uf2` file.
12. Just copy this in your board and it will flashed properly.
13. Rename the file with `.uf2` extension to identify and shareable easily.