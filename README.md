# Proyecto-Simulacion-Octave
This code evaluates how a MRA (Masa-Resorte-Amortiguador) system can be controlled by a PID controller and see its behavior. 

### Recordar
Octave es un software Open Source con funciones similares a las que cuenta MATLAB. 

### Diferencias
El código está escrito con una sintaxis similar a la de MATLAB, solamente que MATLAB requiere que las funciones definidas se encuentren al final del código o en otro archivo, mientras que Octave requiere que se encuentren al inicio, de forma posterior inmediata a los comando clásicos de MATLAB (clc, clear all, close all) 


### Funcionamiento general: 
#### Funciones
Primero se declaran funciones, la función llamada "xp" sirve para caracterizar el sistema de forma abstracta dando valores iniciales a los parámetros que requiere la forma del propio sistema. Igualmente declaramos las ecuaciones propias de un sistema de Segundo Orden. 

Escribimos la función llamada "M" que indica las funciones de transformación geométrica, en este caso, solo son de traslación y de rotación















