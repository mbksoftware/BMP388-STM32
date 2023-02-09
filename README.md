# BMP388-STM32

Reading values example

#include "BMP388.h" // include the library

int32_t Temperature = 0, Pressure = 0, Altitude = 0; // Variables to store data
PRESS_EN_SENSOR_TYPY bmp388Type; //Define sensor model
pressSensorInit(&bmp388Type, hi2c1); //Intitialize sensor

pressSensorDataGet(&Temperature, &Pressure, &Altitude); //Read values into the variables.
