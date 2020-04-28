+++
date = "2020-04-22"
title = "Pyava: a simple emulator launcher written in Python"
+++

Pyava is a simple emulator launcher that I wrote in the october of 2017 using Python (more precisely Python 3), the programming language I was studying at the time.  
It's a portable and convenient menu to run all your games from a single place.  
Its creation was inspired by [Yava](https://github.com/Beluki/Yava), a similar utility written in C# (and the name Pyava itself is the crasis of the words **P**ython and **Yava**).  
The entire project can be found on [GitHub](https://github.com/giacomopoggi/Pyava).

![alt text](/images/pyava-screenshot.png)
*Pyava running on Windows 10*

**Keyboard shortcuts**

| Key    | Use                                              |
| ------ | ------------------------------------------------ |
| Esc    | Close the program.                               |
| Tab    | Change between the left and right panel.         |
| Ctrl+A | Show an information message.                     |
| Ctrl+R | Reload config.ini without closing the program.   |
| Ctrl+S | Set a custom separator for splitting parameters. |

**Configuration**

Pyava is configured using a file named "config.ini". This file contains everything Pyava needs to know about the folders and files it will launch.

Here is an example that generates the screenshot above:
```ini
[Game Boy]
games = C:\Games\Game Boy\
executable = C:\Emulators\BGB\bgb.exe
extensions = .zip, .gb

[Nintendo Entertainment System]
games = C:\Games\Nintendo Entertainment System\
executable = C:\Emulators\Mesen\Mesen.exe
extensions = .7z
parameters = /fullscreen, /DoNotSaveSettings
```
Parameters and extensions are separated by ",". You can set a custom separator using the apposite keyboard shortcut, but it resets to "," every time you select a different platform from the list.