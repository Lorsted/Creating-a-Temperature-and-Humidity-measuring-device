# Creating a Temperature and Humidity measuring device

Written by : Alexander Laskowski – al226nd
 
The purpose of this project is to be able to measure the temperature and humidity and with the help of wifi it will be possible to transfer the measured values to adafruit and later display these values using graphs. This is a project for beginners, and it should take approximately around 3-4 hours to complete the project.

## Objective

I have chosen to build this device because I thought it would be an interesting starting point to IoT and it filled a need which I had at the time as I was curious about the difference between temperature and humidity in rooms connected to each other. These measured values could be used as a starting point as to identify which rooms need to be better ventilated.

## Material

| Name  | Purpose | Name of Vendor | Price (SEK) |
| ------------- | ------------- | ------------- | ------------- |
| Raspberry Pi Pico WH  | Single board microcontroller with wireless function and headers soldered.  | Electrokit  | 109  |
| DHT11  | This sensor measures the Temperature and Humidity of the surrounding.  | Electrokit  | 49  |
| Breadboard | A simple device designed to let you create circuits without the need for soldering.  | Electrokit  | 69  |
| Jumper wires M-M | Used in order to connect the components.  | Electrokit  | 49  |
| Micro USB cable | The cable is used in order to connect the computer to the microcontroller and enabling both charging and the transfer of the program used. | Electrokit  | 39  |


## Computer Setup

For an IDE we use Visual Studio Code. On top of that we will use the PyMakr extension to upload code to the Pico WH. To use the extension we also need to install NodeJS.

### Setting up the environment

1. Install Python if you don't already have it installed.
2. Download and install NodeJS. Make sure to get the current version and not LTS.
3. Download and install the IDE VSCode.
4. Get the PyMakr extension in VSCode.
5. Update firmware on the Raspberry Pi Pico:
   - Download MicroPython firmware. This is a uf2 file. Make sure to get latest one from Releases and not Nightly builds.
   - Connect the micro-USB cable to the Raspberry Pi Pico.
   - While pushing the BOOTSEL button on the board, connect the other end of the micro-USB cable to your computer. After plugging it in you can release the BOOTSEL button.
   - A new drive should pop up in your file system named RPI-RP2 which is the Raspberry Pi Pico storage. Move the uf2, that you downloaded earlier, into this storage.
   - Wait for the board to automatically disconnect and reconnect.

## Putting it together

