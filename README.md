# Template for a Static/Shared/DLL Library Project
* Mainly used this template when working with mingw32 on windows  
* Required tools: Python, Make, And a shell that can run .sh files (e.g mingw32)  
* Python Script included for generating compile_commands.json files
* **If *ANY* directory in the 'setup' recipe is missing, call 'make setup'**
* **COMPILER_BASE_FOLDER** environment variable (Name's pretty self explanatory) **MUST BE DEFINED**
* License: MIT (see license.txt)
#### **Clean Object Files**
    * [Debug]   make cleandbg
    * [Release] make cleanrel
#### **Clean Binaries**
    * [Debug]   make cleanbindbg
    * [Release] make cleanbinrel
#### **Clean Install Folder**
    * [Debug]   make cleaninstalldbg
    * [Release] make cleaninstallrel
#### **Clean Everything**
    * make cleanall
#### **Build Library**
    * [Debug]   make debug   - [Static & Shared Libraries]
    * [Release] make release - [Static & Shared Libraries]
    * [Debug]   make [static/shared]dbg
    * [Release] make [static/shared]rel
#### **Build Library + Clangd Metadata (Don't forget to restart clangd in vscode)**
    * [Debug]   make rec[static/shared]dbg
    * [Release] make rec[static/shared]rel
#### **Install Library at build/install **
    * [Debug]   make installdbg - [Static & Shared Libraries]
    * [Release] make installrel - [Static & Shared Libraries]
    * [Debug]   make install_[static/shared]dbg
    * [Release] make install_[static/shared]rel
