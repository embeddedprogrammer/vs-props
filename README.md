# Visual Studio Property Pages for OpenCV and Matlab
This repository contains some simple examples of property pages for OpenCV and Matlab.

## Adding Property Pages
* Open Visual Studio
* Click View -> Other Windows -> Property Manager
* Right the folder corresponding to your compiler configuration: Debug/Release, Win32/x64
* Click Add Existing Property Sheet
* Navigate to the desired OpenCV or Matlab property pages and add the desired property page
* Note: You may wish to place the property pages in a static directory because Visual Studio will give not very helpful error messages if the path is broken. However, it's not too difficult to manually change the path from the vcxproj file. Additionally, relative paths are supported.
* More information on property pages can be found [here](https://msdn.microsoft.com/en-us/library/669zx6zc.aspx)

## OpenCV Property Pages
* Create and OpenCV_DIR environment variable, as is done in the OpenCV docs instructions linked below
* Make sure you set the OpenCV_DIR to the OpenCV folder (eg. vc14) that corresponds to the correct visual studio version. Note that the visual studio numbering doesn't necessarily correspond to the year. For example, the vc14 folder is for Visual Studio 2015.
* The debug version of OpenCV is very slow. If you need to debug, it is much nicer to compile your own application in debug mode while using the OpenCV release version.
* These property pages were created using instructions found [here](https://docs.opencv.org/2.4/doc/tutorials/introduction/windows_visual_studio_Opencv/windows_visual_studio_Opencv.html)

## Matlab Mex Function Property Page
* This property page was created using the instructions [here](https://www.mathworks.com/help/matlab/matlab_external/compiling-mex-files-with-the-microsoft-visual-c-ide.html)

## Console Property Page
* Keeps the console open after the project finishes running
* This property page was created using the comment by Trevor Robinson [here](https://stackoverflow.com/a/1775870/4307850)

