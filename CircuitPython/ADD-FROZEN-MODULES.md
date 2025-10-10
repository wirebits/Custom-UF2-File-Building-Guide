# Add-Frozen-Modules

# It adds built-in frozen modules while building CircuitPython `uf2` firmware.

# Steps
1. Go to `ports/board_name_folder` folder.
2. Then, go to `boards` folder.
3. Choose your board folder.
4. Go inside the folder.
5. Open `mpconfigboard.mk` file.
6. Just add `FROZEN_MPY_DIRS` lines by just copy from given below list in `mpconfigboard.mk` file.
   - There are the list of built-in frozen modules in proper syntax so that it easily add in `mpconfigboard.mk` file.
   - Each line is for different built-in frozen modules.
   - You can add multiple frozen modules lines as per required by copy these lines in `mpconfigboard.mk` file.
7. Save this file.
8. Done! Build, flash and you don't need to add library files from outside. It is the part of firmware now!

# List of FROZEN_MPY_DIRS
```
FROZEN_MPY_DIRS += $(TOP)/frozen/Adafruit_CircuitPython_AHTx0
```
```
FROZEN_MPY_DIRS += $(TOP)/frozen/Adafruit_CircuitPython_APDS9960
```
```
FROZEN_MPY_DIRS += $(TOP)/frozen/Adafruit_CircuitPython_asyncio
```
```
FROZEN_MPY_DIRS += $(TOP)/frozen/Adafruit_CircuitPython_Bitmap_Font
```
```
FROZEN_MPY_DIRS += $(TOP)/frozen/Adafruit_CircuitPython_BLE
```
```
FROZEN_MPY_DIRS += $(TOP)/frozen/Adafruit_CircuitPython_BLE_Apple_Notification_Center
```
```
FROZEN_MPY_DIRS += $(TOP)/frozen/Adafruit_CircuitPython_BusDevice
```
```
FROZEN_MPY_DIRS += $(TOP)/frozen/Adafruit_CircuitPython_CircuitPlayground
```
```
FROZEN_MPY_DIRS += $(TOP)/frozen/Adafruit_CircuitPython_ConnectionManager
```
```
FROZEN_MPY_DIRS += $(TOP)/frozen/Adafruit_CircuitPython_Crickit
```
```
FROZEN_MPY_DIRS += $(TOP)/frozen/Adafruit_CircuitPython_Display_Shapes
```
```
FROZEN_MPY_DIRS += $(TOP)/frozen/Adafruit_CircuitPython_Display_Text
```
```
FROZEN_MPY_DIRS += $(TOP)/frozen/Adafruit_CircuitPython_DisplayIO_SSD1306
```
```
FROZEN_MPY_DIRS += $(TOP)/frozen/Adafruit_CircuitPython_DotStar
```
```
FROZEN_MPY_DIRS += $(TOP)/frozen/Adafruit_CircuitPython_DRV2605
```
```
FROZEN_MPY_DIRS += $(TOP)/frozen/Adafruit_CircuitPython_DS3231
```
```
FROZEN_MPY_DIRS += $(TOP)/frozen/Adafruit_CircuitPython_ESP32SPI
```
```
FROZEN_MPY_DIRS += $(TOP)/frozen/Adafruit_CircuitPython_FakeRequests
```
```
FROZEN_MPY_DIRS += $(TOP)/frozen/Adafruit_CircuitPython_FocalTouch
```
```
FROZEN_MPY_DIRS += $(TOP)/frozen/Adafruit_CircuitPython_framebuf
```
```
FROZEN_MPY_DIRS += $(TOP)/frozen/Adafruit_CircuitPython_HID
```
```
FROZEN_MPY_DIRS += $(TOP)/frozen/Adafruit_CircuitPython_HTTPServer
```
```
FROZEN_MPY_DIRS += $(TOP)/frozen/Adafruit_CircuitPython_ImageLoad
```
```
FROZEN_MPY_DIRS += $(TOP)/frozen/Adafruit_CircuitPython_IRRemote
```
```
FROZEN_MPY_DIRS += $(TOP)/frozen/Adafruit_CircuitPython_IS31FL3731
```
```
FROZEN_MPY_DIRS += $(TOP)/frozen/Adafruit_CircuitPython_LC709203F
```
```
FROZEN_MPY_DIRS += $(TOP)/frozen/Adafruit_CircuitPython_LED_Animation
```
```
FROZEN_MPY_DIRS += $(TOP)/frozen/Adafruit_CircuitPython_LIS3DH
```
```
FROZEN_MPY_DIRS += $(TOP)/frozen/Adafruit_CircuitPython_LSM6DS
```
```
FROZEN_MPY_DIRS += $(TOP)/frozen/Adafruit_CircuitPython_MIDI
```
```
FROZEN_MPY_DIRS += $(TOP)/frozen/Adafruit_CircuitPython_Motor
```
```
FROZEN_MPY_DIRS += $(TOP)/frozen/Adafruit_CircuitPython_MPU6050
```
```
FROZEN_MPY_DIRS += $(TOP)/frozen/Adafruit_CircuitPython_NeoPixel
```
```
FROZEN_MPY_DIRS += $(TOP)/frozen/Adafruit_CircuitPython_PCF8563
```
```
FROZEN_MPY_DIRS += $(TOP)/frozen/Adafruit_CircuitPython_Pixel_Framebuf
```
```
FROZEN_MPY_DIRS += $(TOP)/frozen/Adafruit_CircuitPython_PortalBase
```
```
FROZEN_MPY_DIRS += $(TOP)/frozen/Adafruit_CircuitPython_ProgressBar
```
```
FROZEN_MPY_DIRS += $(TOP)/frozen/Adafruit_CircuitPython_Register
```
```
FROZEN_MPY_DIRS += $(TOP)/frozen/Adafruit_CircuitPython_Requests
```
```
FROZEN_MPY_DIRS += $(TOP)/frozen/Adafruit_CircuitPython_RFM9x
```
```
FROZEN_MPY_DIRS += $(TOP)/frozen/Adafruit_CircuitPython_RFM69
```
```
FROZEN_MPY_DIRS += $(TOP)/frozen/Adafruit_CircuitPython_SD
```
```
FROZEN_MPY_DIRS += $(TOP)/frozen/Adafruit_CircuitPython_seesaw
```
```
FROZEN_MPY_DIRS += $(TOP)/frozen/Adafruit_CircuitPython_SHT4x
```
```
FROZEN_MPY_DIRS += $(TOP)/frozen/Adafruit_CircuitPython_SimpleIO
```
```
FROZEN_MPY_DIRS += $(TOP)/frozen/Adafruit_CircuitPython_SimpleMath
```
```
FROZEN_MPY_DIRS += $(TOP)/frozen/Adafruit_CircuitPython_SSD1306
```
```
FROZEN_MPY_DIRS += $(TOP)/frozen/Adafruit_CircuitPython_SSD1680
```
```
FROZEN_MPY_DIRS += $(TOP)/frozen/Adafruit_CircuitPython_ST7789
```
```
FROZEN_MPY_DIRS += $(TOP)/frozen/Adafruit_CircuitPython_Thermistor
```
```
FROZEN_MPY_DIRS += $(TOP)/frozen/Adafruit_CircuitPython_Ticks
```
```
FROZEN_MPY_DIRS += $(TOP)/frozen/Adafruit_CircuitPython_UC8151D
```
```
FROZEN_MPY_DIRS += $(TOP)/frozen/Adafruit_CircuitPython_Wave
```
```
FROZEN_MPY_DIRS += $(TOP)/frozen/Adafruit_CircuitPython_Wiznet5k
```
```
FROZEN_MPY_DIRS += $(TOP)/frozen/CircuitPython_AXP313A
```
```
FROZEN_MPY_DIRS += $(TOP)/frozen/CircuitPython_AXP2101
```
```
FROZEN_MPY_DIRS += $(TOP)/frozen/CircuitPython_BMA423
```
```
FROZEN_MPY_DIRS += $(TOP)/frozen/circuitpython_ef_music
```
```
FROZEN_MPY_DIRS += $(TOP)/frozen/circuitpython_picoed
```
```
FROZEN_MPY_DIRS += $(TOP)/frozen/circuitpython-pcf85063a
```
```
FROZEN_MPY_DIRS += $(TOP)/frozen/circuitpython-stage
```
```
FROZEN_MPY_DIRS += $(TOP)/frozen/mixgo_cp_lib
```
```
FROZEN_MPY_DIRS += $(TOP)/frozen/pew-pewpew-lcd
```
```
FROZEN_MPY_DIRS += $(TOP)/frozen/pew-pewpew-standalone-10.x
```