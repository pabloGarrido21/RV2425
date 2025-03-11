# Practica 1 Bases de un modelo

Seguir el pdf está bien, pero hay que hacer ciertas modificaciones

1.) hay que añadir los archivos "glew32.dll","FreeImage.dll" y "glfw3.dll" a X64/Debug

 2.) en la clase CGApplication.cpp hay que cambiar una cosa en el método swapFullScreen():

    else
    {
      fullScreen = false;
      glfwSetWindowMonitor(window, nullptr, windowXpos, windowYpos, 
                                            windowWidth, windowHeight, nullptr);
    }

  Ese último nullptr, hay que cambiarlo por un 0

       else
    {
      fullScreen = false;
      glfwSetWindowMonitor(window, nullptr, windowXpos, windowYpos, 
                                            windowWidth, windowHeight, 0);
    }
