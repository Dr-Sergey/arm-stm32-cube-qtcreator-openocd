
# Create a project with STM32CubeMX for QtCreator
Below we will create a virtual comport (CDC) project with STM32CubeMX and import project to QTCreateor. The final project you can find in the usb_vcp folder in this repository.
  
1. Run STM32CubeMX and start **New Project**  
![run_cube](img/cube_start.png)  

2. Select **STM32F4DISCOVERY** for the project as shown on the picture 
![select_board](img/cube_select_board.png) 

3. Confure MCUs pins
![config_pins1](img/cube_config_pins_1.png) 
![config_pins2](img/cube_config_pins_2.png) 

4. Rifine clock configration
![clock_config](img/cube_clock_config.png) 

5. Configure **Middlewares** as shown on the picture
![config_midlewares](img/cube_config.png) 

6. Go to menu **Project -> Settings** and configure the project. Here we use **Makefile** as toolchain. This important for importing into QtCreator.
![config_project](img/cube_settings.png)  
also configure settings for **Code Generator**
![config_code_gen](img/cube_code_gen_settings.png) 

7. Close **Project Settings**  window by click on Ok. And run **Generate Code** in **Project** menu.

8. Run **QtCreator** and goto menu **File -> New File or Porject**. Select **Import Project -> Import Existing Project**
![qt_new_project](img/tut_import_project.png) 

9. Enter project name **usb_vcp** and location of project generated in previus step.
![qt_import_project](img/tut_import_location.png)  

10. Select all files to be imported and click **Next**
![qt_select_files](img/tut_import_files.png)  
click **Finish**  
![qt_import_summary](img/tut_import_summary.png)  

11. Now we can see the opened project in QtCreator IDE
![qt_project](img/tut_project.png)  
