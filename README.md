## Installation Guide for MinGW
1. _Install MinGW_, cmake, ninja

   Suppose MinGW is installed to directory C:/MinGW
   Add C:/MinGW/bin to the system Path variable
   
2. _Install glew_

   Build glew using the following commands:
      ```
      $cd dependencies
      $unzip glew-2.1.0.zip
      $cd glew-2.1.0/build/cmake
      $cmake -G Ninja .
      $ninja
      ```
   Go to directory lib, and copy libglew32.a & libglew32.dll.a to C:/MinGW/lib.
   Go to directory bin, and copy glew32.dll to C:/MinGW/bin.
   Copy glew-2.1.0/include/GL to C:/MinGW/include manually.

3. _Install glfw_

   Build glfw using the following commands:
      ```
      $cd dependencies
      $unzip glfw-3.2.1
      $cd glfw-3.2.1
      $cmake -G Ninja .
      $ninja
      ```
   Copy src/libglfw3.a to C:/MinGW/lib.
   Copy glfw-3.2.1/include/GLFW to C:/MinGW/include.

4. _Remaining steps_

   Copy gvimrc to the installation directory of gvim, and rename it as _gvimrc.
   Copy ```stb_image.h``` to C:/MinGW/include.
   Unzip rapidjson.zip and copy rapidjson to C:/MinGW/include.

