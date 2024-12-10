A version of RTKLIB based on rtklibexplorer. The main focus of the evolutions have been to improve positioning performance, especially when using long-baseline (i.e > 10km distance) or VRS for the reference station. 
This software is provided “AS IS” without any warranties of any kind.

This fork has not been especially tailored to work with any of GMV's products and is still valid for general-purpose positioning.

Releases with Windows executables are avaiable at https://github.com/GMV-APS/RTKLIB/releases

Tutorials for this code, and sample GPS data sets from rtkexplorer team are available at http://rtkexplorer.com/  

The latest version of the user manual by rtklibexplorer team is at: https://rtkexplorer.com/pdfs/manual_demo5.pdf

   
WINDOWS: To build and install code for with Windows Embarcadero compiler:

GUIs: 
1) Build executables with app/winapp/rtklib_winapp.groupproj project file 
2) Install executables and DLLs to ../RTKLIB/bin by runnning app/winapp/install_winapp.bat

CUIs:
1) Build executables with app/consapp/rtklib_consapp.groupproj project file 
2) Install executables to ../RTKLIB/bin by runnning app/consapp/install_consapp.bat



LINUX: To build and install code

CUIs:
1) cd app/consapp/<appName>/gcc
2) make

GUIs (Qt based - available but not fully supported):
1) cd app/qtapp
2) qmake
3) make
4) ./install_qtapp

The linux GUI files have been updated but are not fully functional. 
In general, GUIs have been adapted but not fully validated as their linux CUIs counterparts have.
Especial care has to be taken when using RTKPOST as it cannot be fully configurable even when loading a configuration file. Usage is discouraged in favour of its CUI counterpart rnx2rtkp.
