# What is QEDA

QEDA is a tool aimed to make electronic devices development easy and fun.

## Structure

QEDA consists of:

* [QEDA CLI](/cli/) — a command-line utility which provides a simple but highly customizable mechanism for creating electronic component libraries for use in EDA software.

  This is the engine of QEDA.

* [QEDA Library](https://github.com/qeda/lib) — an open, free, and constantly growing repository of ready-for-use electronic components.

  This is the fuel of QEDA.

## Features

* **Simple electronic component definition**

  Even if a component is not in a library yet, you simply define it by creating or editing a short and human readable text file in [YAML](https://yaml.org) format.

* **Flexible customization**

  We try to take into account all settings you would like to adjust and grouped them to easily accessible parameters.

* **Compliance with your corporate style**

  All schematic symbols and land patterns will share common style according to your specific settings. If your style changes the only thing you need to do is to regenerate libraries with your new settings. You may adapt the look of schematic symbols to the actual standard of your company or country.

* **Accordance to leading industry standards (IPC, JEDEC, JEITA)**

  We use the latest IPC-7351B guidelines to create land patterns. Housing specifications are partially borrowed from respective JEDEC and JEITA standards.
