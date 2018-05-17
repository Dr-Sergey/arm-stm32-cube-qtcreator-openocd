# QtCreator environment for STM32 32-bit ARM Cortex MCUs

&nbsp;&nbsp;&nbsp;&nbsp;This repository is a tutorial and an example how to setup QtCreator environment for bare metal devices (STM32 ARM).
This readme will describe a tutorial on how to tune up QtCreator, using OpenOCD for on-chip debugging, create a project with STM32CubeMX and import it into QtCreator. Here you can find the final project (usb_vcp) for STM32F4DISCOVERY board.

### Prerequisites
- QtCreator 
- ARM GCC
- GDB 
- OpenOCD
- STM32CubeMX

**QtCreator**: 
> Download from QT [site](https://www.qt.io) and install.

**ARM GCC**:
> Open in terminal and run:  
&nbsp;&nbsp;&nbsp;&nbsp;_sudo apt-get install gcc-arm-none-eabi_  
> __or download__ and extract it from [launchpad](https://launchpad.net/gcc-arm-embedded/+download)

**GDB**:
> There is need an arm gdb with python scripting support.  
> Download it from the [download archives](http://ftp.gnu.org/gnu/gdb/).  
> Extract the source archive.  
> Open in terminal and run:  
&nbsp;&nbsp;&nbsp;&nbsp;_./configure --with-python --target=arm-elf_  
&nbsp;&nbsp;&nbsp;&nbsp;_make_  
> When compilation done you can find the gdb executable in the main directory.  
> __Another way__ is to use _arm-none-eabi-gdb-py_ from gcc toolchain.  

**OpenOCD**:
> Open in terminal and run:  
&nbsp;&nbsp;&nbsp;&nbsp;_sudo apt-get install openocd_  
> or download and [install](https://gnu-mcu-eclipse.github.io/openocd/install/) from [OpenOCD site](http://openocd.org/)

**STM32CubeMX**: 
> Download from STMicroelectronics [site](http://www.st.com/en/development-tools/stm32cubemx.html) and install.

All is running on Linux Ubuntu 16.04. It should be similar for other Linux distributions or versions.

# Tutorials and Examples
- [Setting up QtCreator environment](set_qtc.md)
- [OpenOCD for in-system programming](openocd.md)
- [Create a project with STM32CubeMX for QtCreator](prj_cube_qt.md)
- [On-chip debugging STM32 with QtCtreator](debug.md)
