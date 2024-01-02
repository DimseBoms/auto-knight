# KDE Plasma automatic night theme switcher
auto-knight is a shell script that automatically switches between light and dark themes in KDE Plasma. It uses the color temperature settings from KDE's Night Color feature to determine when to switch themes.

It is intended to be light weight.

## Dependencies
* qdbus-qt5: A tool for sending and reading DBus messages and values. This is used to get the current color temperature from KDE's Night Color feature.
* kreadconfig5: A tool for reading KDE configuration files. This is used to get the default color temperature from the Night Color settings.
* dbus-monitor: A tool for monitoring DBus messages. This is used to detect changes in the target color temperature.
* grep: A tool for filtering text. This is used to filter the output of dbus-monitor for messages about the target color temperature.

## Installation
To use Auto-Knight, you need to have the above dependencies installed. You can then download the script, make it executable and add it to the login script via autostart.

## Customization
You can customize the light and dark themes used by the script by modifying the light_theme and dark_theme variables at the top of the script.
