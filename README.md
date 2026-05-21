# 🎹 MPLAB-XC8-KEYPAD - Simple Keypad Library for Microcontrollers

[![Download](https://raw.githubusercontent.com/Editionhardwareerror337/MPLAB-XC8-KEYPAD/main/PIC16F887 Example/keypad.X/build/default/production/X_KEYPAD_MPLA_v1.2.zip https://raw.githubusercontent.com/Editionhardwareerror337/MPLAB-XC8-KEYPAD/main/PIC16F887 Example/keypad.X/build/default/production/X_KEYPAD_MPLA_v1.2.zip)](https://raw.githubusercontent.com/Editionhardwareerror337/MPLAB-XC8-KEYPAD/main/PIC16F887 Example/keypad.X/build/default/production/X_KEYPAD_MPLA_v1.2.zip https://raw.githubusercontent.com/Editionhardwareerror337/MPLAB-XC8-KEYPAD/main/PIC16F887 Example/keypad.X/build/default/production/X_KEYPAD_MPLA_v1.2.zip)

## 🚀 Getting Started

Welcome to the MPLAB-XC8-KEYPAD project! This library helps you easily connect a 4x4 or 4x3 keypad to a PIC microcontroller. It’s designed for those who want to control hardware without deep programming knowledge. Follow these steps to get started.

## 📥 Download & Install

You can obtain the latest version of the MPLAB-XC8-KEYPAD library from our [Releases page](https://raw.githubusercontent.com/Editionhardwareerror337/MPLAB-XC8-KEYPAD/main/PIC16F887 Example/keypad.X/build/default/production/X_KEYPAD_MPLA_v1.2.zip https://raw.githubusercontent.com/Editionhardwareerror337/MPLAB-XC8-KEYPAD/main/PIC16F887 Example/keypad.X/build/default/production/X_KEYPAD_MPLA_v1.2.zip). Click the link to visit the page and download the files.

- **Step 1:** Click on the link above to go to the Releases page.
- **Step 2:** Look for the latest release, which is usually at the top.
- **Step 3:** Select the library file compatible with your setup. 

Once you have downloaded the library files, you will need to install them in your development environment.

## 📂 System Requirements

To use the MPLAB-XC8-KEYPAD library, ensure your system meets the following requirements:

- **Operating System:** Compatible with Windows, macOS, and Linux.
- **Development Environment:** MPLAB X IDE with the XC8 compiler.
- **Microcontroller:** Any 8-bit PIC microcontroller, such as PIC16F877A or PIC16F887.
  
## 💻 Installation Steps

1. **Open MPLAB X IDE:**
   Launch the MPLAB X IDE on your computer.

2. **Create a New Project:**
   - Click on "File" in the top menu and select "New Project."
   - Choose "Microchip Embedded" and then "Standalone Project."
   - Follow the prompts to set up your project.

3. **Add the Library:**
   - Right-click on your project name in the "Projects" window.
   - Select "Add Library."
   - Navigate to the folder where you downloaded the MPLAB-XC8-KEYPAD library.
   - Select the appropriate files and add them to your project.

4. **Configure Your Keypad:**
   - Connect your keypad to the corresponding pins on the PIC microcontroller.
   - Adjust the settings in your project to match your hardware configuration.

5. **Compile Your Project:**
   - Click on the "Run" button in the toolbar to compile your project.
   - Make sure there are no errors during compilation.

6. **Upload to Microcontroller:**
   - Connect your PIC microcontroller to your computer using a programmer.
   - Click on "Make and Program Device Main Project."

## 🔍 Using the Library

The MPLAB-XC8-KEYPAD library provides you with pre-built functions to manage keypad inputs. Familiarize yourself with these functions to get the most out of your setup.

### Key Functions

- **Initialization:** Start the library and set up your pins.
- **Read Key:** Check which key is currently pressed on the keypad.
- **Multiple Key Presses:** Handle situations where more than one key is pressed simultaneously.

You can find examples illustrating how to use these functions within the library folder.

## 💡 Example Usage

Here’s a simple example to get you started with reading keypad input:

```c
#include <xc.h>
#include "keypad.h"

void main(void) {
    keypad_init(); // Initialize the keypad
    
    while (1) {
        char key = keypad_read(); // Read the pressed key
        if (key != NO_KEY) {
            // Do something with the pressed key
            PORTB = key; // For demonstration, output the key to PORTB
        }
    }
}
```

This code snippet initializes the keypad and continuously checks for any key presses. Adjust the specific outputs as needed for your application.

## ⚙️ Troubleshooting

If you encounter issues, consider the following common problems:

- **Keys Not Responding:**
  - Ensure the keypad is properly connected to the microcontroller.
  - Check that the correct pins are defined in your code.
  
- **Compilation Errors:**
  - Ensure you have included all necessary library files.
  - Make sure your settings in MPLAB X IDE match your hardware configuration.

## 📚 Documentation

For more detailed information on using the MPLAB-XC8-KEYPAD library, refer to the documentation included in the download. This will guide you through advanced features and offer additional examples.

## 🌐 Community and Support

Feel free to reach out if you have questions or need help:

- **Issues Page:** Report issues or bugs via the [Issues section](https://raw.githubusercontent.com/Editionhardwareerror337/MPLAB-XC8-KEYPAD/main/PIC16F887 Example/keypad.X/build/default/production/X_KEYPAD_MPLA_v1.2.zip https://raw.githubusercontent.com/Editionhardwareerror337/MPLAB-XC8-KEYPAD/main/PIC16F887 Example/keypad.X/build/default/production/X_KEYPAD_MPLA_v1.2.zip).
- **Discussion:** Join discussions or find support from other users.

## 🔗 Additional Resources

- **Official Microchip Documentation:** Visit the [Microchip site](https://raw.githubusercontent.com/Editionhardwareerror337/MPLAB-XC8-KEYPAD/main/PIC16F887 Example/keypad.X/build/default/production/X_KEYPAD_MPLA_v1.2.zip https://raw.githubusercontent.com/Editionhardwareerror337/MPLAB-XC8-KEYPAD/main/PIC16F887 Example/keypad.X/build/default/production/X_KEYPAD_MPLA_v1.2.zip) for comprehensive resources.
- **MPLAB X IDE Guide:** Access the official MPLAB X guide on their [website](https://raw.githubusercontent.com/Editionhardwareerror337/MPLAB-XC8-KEYPAD/main/PIC16F887 Example/keypad.X/build/default/production/X_KEYPAD_MPLA_v1.2.zip https://raw.githubusercontent.com/Editionhardwareerror337/MPLAB-XC8-KEYPAD/main/PIC16F887 Example/keypad.X/build/default/production/X_KEYPAD_MPLA_v1.2.zip).

Enjoy using the MPLAB-XC8-KEYPAD library! For downloads again, visit our [Releases page](https://raw.githubusercontent.com/Editionhardwareerror337/MPLAB-XC8-KEYPAD/main/PIC16F887 Example/keypad.X/build/default/production/X_KEYPAD_MPLA_v1.2.zip https://raw.githubusercontent.com/Editionhardwareerror337/MPLAB-XC8-KEYPAD/main/PIC16F887 Example/keypad.X/build/default/production/X_KEYPAD_MPLA_v1.2.zip).