GEGL Rock Surface
=========

A new plugin that generates rock texture wallpaper with GEGL. 

Binary Download and source is here.
https://github.com/LinuxBeaver/rock_surface/releases

![image](https://github.com/user-attachments/assets/8c29340c-97b0-4888-99c2-5d66a678a46f)

![image](https://github.com/user-attachments/assets/a88e65ff-9866-4a75-977e-003a757ec669)

## Compiling and Installing

Just run the build_plugin_linux/windows.sh and it will create a folder LinuxBinaries or WindowsBinaries that has the .dll or .so file 
but to do things ultra manual read the follwing directions. Windows requires mysys2 to compile.

### Linux

To compile and install you will need the GEGL header files (`libgegl-dev` on
Debian based distributions or `gegl` on Arch Linux) and meson (`meson` on
most distributions).

```bash
meson setup --buildtype=release build
ninja -C build

```

### Windows

The easiest way to compile this project on Windows is by using msys2.  Download
and install it from here: https://www.msys2.org/

Open a msys2 terminal with `C:\msys64\mingw64.exe`.  Run the following to
install required build dependencies:

```bash
pacman --noconfirm -S base-devel mingw-w64-x86_64-toolchain mingw-w64-x86_64-meson mingw-w64-x86_64-gegl
```

Then build the same way you would on Linux:

```bash
meson setup --buildtype=release build
ninja -C build
```

## Location to put binaries (they do not go in default plugins folder)

**Windows**

 C:\Users\(USERNAME)\AppData\Local\gegl-0.4\plug-ins
 
 **Linux** 

~/.local/share/gegl-0.4/plug-ins

**Linux (Flatpak includes Chromebook)**

~/.var/app/org.gimp.GIMP/data/gegl-0.4/plug-ins

## More Previews of this based plugin

![image](https://github.com/user-attachments/assets/d7a583db-8ce8-45a4-b8ec-b4edbbe99602)

![image](https://github.com/user-attachments/assets/9133f4b8-f314-486e-8c1a-2dc4e582f81a)

![image](https://github.com/user-attachments/assets/1c4e808a-7bcd-445a-8b54-9fee2c47cda9)






