# Proyecto-Simulacion-Octave
This code evaluates how a MRA (Masa-Resorte-Amortiguador) system can be controlled by a PID controller and see its behavior. 

### Recordar
Octave es un software Open Source con funciones similares a las que cuenta MATLAB. 

### Diferencias
El código está escrito con una sintaxis similar a la de MATLAB, solamente que MATLAB requiere que las funciones definidas se encuentren al final del código o en otro archivo, mientras que Octave requiere que se encuentren al inicio, de forma posterior inmediata a los comando clásicos de MATLAB (clc, clear all, close all) 


### Funcionamiento general: 
#### Funciones
Primero se declaran funciones, la función llamada **xp** sirve para caracterizar el sistema de forma abstracta dando valores iniciales a los parámetros que requiere la forma del propio sistema. Igualmente declaramos las ecuaciones propias de un sistema de Segundo Orden. 

Escribimos la función llamada **M** que indica las funciones de transformación geométrica, en este caso, solo son de traslación y de rotación. Las transformaciones solamente estarán dadas para el plano 2D, por lo que las matrices serán de **3x3**

### Cuerpo del código
Comenzamos definiendo en un espacio geométrico de forma puntual y simple las entidades que serán involucradas en el código.

**Masa** 
> Compuesta por 5 puntos y una distancia de una unidad entre ellos

**Rueda**
> Compuesta por la función de un círculo y 3 líneas que se desprenden desde el centro hacia la circunferencia.

**Resorte**
> Dado por puntos en una geometría abrierta, forma de ZigZag con la finalidad de hacerlo lo más simple representativamente. 

Posteriormente definimos el tiempo y su intervalo 
```
h = 0.5; ti = 0; tff = 70;
T = (ti:h:tff);
```

Luego colocamos el método para hacer la integración mediante **odeset**, parte importante del funcionamiento correcto del controlador. 


### Evaluación 
Primero evaluamos las funciones de transformación dando valores iniciales y de posición.

Fijamos los exis del sistema de ploteo. 

Y finalmente evaluamos todo el sistema de animación con el comportamiento que nos dicta la recta del controlador. 
















