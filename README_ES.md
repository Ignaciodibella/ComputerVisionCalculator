# Computer Vision Calculator
Calculadora controlada por gestos usando Computer Vision en Python.
<div align="center">
     <img src = "https://github.com/Ignaciodibella/ComputerVisionCalculator/blob/main/cvcalc.gif">
</div>

<br>

<div align="center">
     <img src = "https://github.com/Ignaciodibella/ComputerVisionCalculator/blob/main/handrecognition.png" width = 507 height = 284>
</div>

### 💡 Cómo usarlo:
1. Descargar el archivo `CVCalculator.py`.
2. Ver la sección de **Requerimientos** para los detalles de instalación.
3. Una vez en funcionamiento, se abrirá una ventana mostrando lo que ve la camara de la computadora. 
4. El dedo índice servirá de mouse. 
  <br>La linea que conecta los dedos índice y mayor permite medir la distancia entre ellos. Si se juntan estarán simulando un click. 
  <br>**Tener en cuenta que mientras mas cerca se tenga la mano de la pantalla, menor sensibilidad tendrá el clic y, al alejar la mano se tendrá mayor sensibilidad**
5. Hay dos teclas especiales en el teclado de la calculadora mostrada:
  <br>**D:** Usada como simulador de la tecla `Del` (borra el último número u operador ingresado),
  <br>**C:** Usada como simulador de la tecla `Clear`, limpiando el contenido de la pantalla de la calculadora.
6. Para tener en cuenta:
   <br> Ingresar 2**3 implica una operación de potencia, siendo el resultado en este ejemplo 8 (base, exponente).
   <br> Dos signos negativos consecutivos resultarán en una suma (5 - - 5 = 10)
   <br> algo similar pasa si se mezclan +/-, lo que resulta en una resta (5 +- 2 = 3)

### ⚠️Requerimientos: 
Es necesario instalar lo siguiente:
- `cvzone` (para este proyecyo usé la versión 1.5.6)
- `opencv-python` (para este proyecyo usé la versión 4.7.0.72)
- `mediapipe`

El proyecto fue creado usando `Python 3.9`.

### 🛠️Configuración:
- en la linea 82 se muestra el comando: `#print(length)`
<br> Si se descomenta y ejecuta el programa, al juntar o alejar los dedos índice y mayor entre sí, una serie de prints se van a ir mostrando por la consola, mostrando la distancia entre ellos.
<br> Esto está pensado para poder ajustar o calibrar la sensibilidad del clic, pero la configuración actual debería funcionar correctamente.
<br> Sin embargo, si es necesario pueden ajustar esto en la linea 84 `if length < 47:`

<div align="center">
<img src ="https://github.com/Ignaciodibella/ComputerVisionCalculator/blob/main/length.PNG">
</div>
