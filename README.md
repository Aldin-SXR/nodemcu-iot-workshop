# NodeMCU Workshop

## NodeMCU & ESP8266

__NodeMCU__ is a popular and inexpensive development board, based on the widely explored __ESP8266__ microcontroller unit by _Espressif_. It offers WiFi networking capabilities (enabling it to be used as an access point, station or a Web server), Arduino-like hardware I/O as well as a myriad other stand-alone features, allowing it to form an excellent basis for an IoT platform.
  
As an open-source, full development board centered around ESP8266, NodeMCU includes an additional USD to Serial UART adapter, a micro-USB programming port and a 3.3V regulator, making it easy to connect to your computer, install the necessary drivers and begin developement.

Read more about NodeMCU and ESP8266 on the [http://42bots.com/esp8266/nodemcu-esp8266-iot-development-board-overview/](following link).
  
## Project Setup

Follow the steps outlined in this section to install the software necessary for the workshop.

### VSCode
__Visual Studio Code__ is a lightweight but powerful source code editor which runs on your desktop and is available for Windows, macOS and Linux.

It comes with support for a number of programming languages (C/C++ included), and is easy to set up and customize with extensions. In this workshop, we will use VSCode instead of the "standard" choice of Arduino IDE, as it offers a great extension [ihttps://platformio.org/](PlatformIO) (which will handle all our NodeMCU library setup and installation needs).

You can install VSCode by downloading the appropriate version for your system from [https://code.visualstudio.com/](the official link).

### PlatformIO

__PlatformIO__ is an open source cross-platform ecosystem for IoT development, featuring an IDE, a unified debugger, remote unit testing and firmware updates. It supports over 600 embedded boards (ESP8266 included), without external dependencies to a system software. It is available as an extension to _VSCode_ and _Atom_, offering easy adaptability and high customizability.

#### Why PlatformIO?

It is possible to write code for ESP8266 (NodeMCU) in a standard Arduino IDE. However, using PlatformIO saves us the hassle of having to manually install different libraries and drivers required for the board, allowing us to be set up as soon as possible. 

Moreover, PlatformIO is a fully-featured IDE, offering numerous other functionalities lacking in Arduino IDE, such as code completion and linting, debugging, testing and much more.

- _Installation_: 
    1. After installing VSCode, navigate to the `Extensions` tab on the left side of the IDE (or use the shortcut `Ctrl+Shift+X`), and search for "PlatformIO".
    
    ![Find "PlatformIO" extension](./img/platformio-install.png)

    2. Once you press `Install`, wait for the process to be completed. Soon afterwards, the bottom window `Output` will open, informing you that "PlatformIO Core" is being installed. __Do not__ close this window and wait for the setup to finish. 
    3. After the core is installed, you will be prompted to `Reload` the window. 

    ![Wait for the installation to finish](./img/platformio-install-2.png)

    4. Once the IDE restarts, you will be greeted by the PlatformIO home screen. You are now ready to create your first project.

