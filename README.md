# Apuntes---Primera-Semana
Apuntes control de movimiento primer corte, Primera Semana
# CONTROL DE MOVIMIENTO
Ademas de reconocer que es control de movimiento, conoceremos muchas de sus aplicaciones en la industria.
>🔑 *Definición:* Se basa en el control del movimiento mecánico de un sistema con carga

## 1. Ejes de Movimiento
Los también denominados axis, se asocian a cada movimiento que generen los actuadores involucrados en un sistema especifico. Generalmente los sistemas de control de movimiento tienen más de un eje de movimiento, y por cada uno de los axis que compongan al sistema podemos llegar a controlar variables como: posición, velocidad, torque y asceleración; la finalidad de controlar al menos una de estas variables en cada eje es para garantizar la sincronica del proceso que se este llevando acabo, y con ellos tener mejores resultados en los productos o procesos. 

## 2. Historia del Control de Movimiento

A lo largo de la historia podemos encontrar multiples maquinas en la industria, que desempeñan diversas tareas como lo eran máquinas dobladoras o máquinas etiqueteadoras. En los casos expuestos anteriormente, las máquinas solo contaban con un motor con un eje largo que utilizaba engranajes y mecanismos para modificar trayectorias, velocidaddes y acelaraciones en diferentes ejes, manteniéndolos sincronizados con el motor principal. Sin embargo, han caído en desuso debido a su falta de flexibilidad y al alto costo y complejidad de su mantenimiento.

### 2.1. Componentes

Los diferentes componentes que se utilizan dentro del sistema de control de movimiento dependen de la funcionalidad que se le vaya a dar al mecanismo; dentro de estos encontramos drivers de potencia, actudaores, interfaces humanas entre otras. A continuacion entramos en detalle de cada uno de los elementos que componen al sistema.

* Interfaz Humano - Máquina: Es el medio a través del cual una persona interactúa con una máquina o sistema, permitiendo el control y monitoreo de sus funciones. Puede incluir pantallas táctiles, botones, teclados, luces y software especializado. ![](https://github.com/MariaFernandaOrtiz-111449/Apuntes---Primera-Semana/blob/e9fa32c35e96e5ddc59e32fea7918aa31ce8db29/HMI.png)

* Controlador de movimiento: Componente que gestiona y coordina el movimiento de motores en sistemas automatizados. Se encarga de generar señales precisas para controlar velocidad, posición y aceleración, permitiendo un funcionamiento eficiente y sincronizado en aplicaciones como robótica, CNC y automatización industrial. ![](https://github.com/MariaFernandaOrtiz-111449/Apuntes---Primera-Semana/blob/3029c00e61f50720e01463f7931400106c433b29/Controlador%20de%20movimiento.png)

* Actuadores: Dispositivos que convierten una señal de control en movimiento o acción física. Pueden ser eléctricos, hidráulicos o neumáticos y se utilizan para realizar tareas como mover un motor, accionar una válvula o girar un mecanismo en sistemas automatizados. ![](https://github.com/MariaFernandaOrtiz-111449/Apuntes---Primera-Semana/blob/3829a7559e04368c8e27dfcec81313c58c7d80d1/Actuadores.png)

* Mecanismos de Transmisión: Sistemas que transfieren movimiento y fuerza desde un componente a otro en una máquina. Pueden modificar velocidad, torque y dirección, e incluyen engranajes, poleas, correas, cadenas y tornillos sin fin, entre otros. ![](https://github.com/MariaFernandaOrtiz-111449/Apuntes---Primera-Semana/blob/9e45b3b50aa59837af4a97075f572527abd2a27b/Mecanismos%20de%20transmisi%C3%B3n.png)

* Sensores: Dispositivos que detectan cambios en el entorno y convierten esa información en señales eléctricas para su procesamiento. Se usan en automatización, robótica y electrónica para medir variables como temperatura, luz, presión, movimiento y posición. ![](https://github.com/MariaFernandaOrtiz-111449/Apuntes---Primera-Semana/blob/555801acae4a65de19998b7531878791a79b358c/Sensores.png)
  
## 3. Características del control

El control de movimiento cuenta con ciertas carácterísticas que le hacen prioritario como análisis del movimiento. Al aplicar movimiento a una carga, se genera una fuerza negativa que afecta la velocidad del motor, conocida como offset de velocidad. Para minimizar esta perturbación, es crucial controlar el torque de manera rápida y suave. Además, la dinámica de la velocidad debe ser precisa para lograr trayectorias curvas exactas. Un diseño eficiente del driver de potencia es fundamental para optimizar el consumo energético y prolongar la vida útil del motor y la electrónica.

### Control cascada

El control de cascada es una estrategia de control en la que se usan dos o más lazos anidados para mejorar la respuesta del sistema. Un controlador principal regula la variable principal y envía su salida a un controlador secundario, que ajusta una variable intermedia para mayor precisión y estabilidad, reduciendo perturbaciones y mejorando el desempeño. ![](https://github.com/MariaFernandaOrtiz-111449/Apuntes---Primera-Semana/blob/bf72f46053468b2583775e90e2e437547f8ffdb6/Control%20cascada.png)

## 4. Ejemplos

El uso del control cascada está muy ligado a la industria debido a que mejora la estabilidad y precisión del sistema al reducir el impacto de perturbaciones. Permite una respuesta más rápida y eficiente, ya que el controlador secundario corrige variaciones antes de que afecten la variable principal. Es común en procesos con inercias grandes, como control de temperatura, presión y velocidad en maquinaria industrial.

A continuación observaremos diferentes usos que se les da al control cascada dentro de la industria:

### Transporte
* Cadenas de suministros automatizadas: el control en cascada se usa para optimizar el flujo de materiales y productos. Un controlador principal gestiona la producción y la logística general, mientras que controladores secundarios ajustan variables como velocidad de transportadores, tiempos de almacenamiento y distribución. Esto mejora la eficiencia, reduce retrasos y minimiza interrupciones en el proceso.
  ![](https://github.com/MariaFernandaOrtiz-111449/Apuntes---Primera-Semana/blob/c249450fa8e7f916ab7f95022005b6a2cf6859f4/Cadenas%20de%20suministros%20automatizadas.png)

### Productos alimenticios
*El control en cascada se utiliza para garantizar calidad y eficiencia en procesos como pasteurización, horneado y envasado. Un controlador principal regula variables clave como temperatura o presión, mientras que controladores secundarios ajustan parámetros intermedios, como el flujo de vapor o la velocidad de cintas transportadoras. Esto permite un control preciso, reduciendo desperdicios y asegurando uniformidad en el producto final. ![]()
## 5. Ecuaciones
Para la edición de ecuaciones debe utilizar la etiqueta '$$' al comienzo y final de la ecuación para que la ecuación quede centrada ocupando una línea. Si se quiere que la ecuación quede integrada en el texto debe utilizar la etiqueta '$' al comienzo y final de la ecuación. Las ecuaciones pueden ser editadas utilizando el código LATEX, en el siguiente enlace encuentran un editor de ecuaciones que les genera el código. http://www.alciro.org/tools/matematicas/editor-ecuaciones.jsp . Sin embargo hay muchas otras herramientas que pueden utilizar para esto.

💡**Ejemplo 1:** si se va a representar la ecuación de la ley de Ohm se puede mostrar así $R=\frac{V}{I}$ o también,

$$R=\frac{V}{I}$$

## 6. Figuras
Todas las figuras que incluya deben ser generadas por ustedes, **no utilizar las figuras de las presentaciones**. Para incluir figuras puede seguir los siguientes pasos:
* Primero escribimos ![]().
* Después escribimos, dentro de los corchetes, el texto alternativo. Este es opcional y solo entra en acción cuando no se puede cargar la imagen correctamente.
* Después escribimos, dentro de los paréntesis, la ubicación del archivo (ya sea una url o una ubicación dentro de algun folder local). Se recomienda poner las imágenes en una carpeta que se llame imágenes dentro del repositorio github para que no tengan problemas al cargar las imágenes.

💡**Ejemplo 2:**

![Figura de prueba](images/plantilla/Captura2.PNG)

Figura 1. Figura de prueba

Incluya la respectiva etiqueta a modo de descripción de la figura y mantenga numeración consecutiva para todas las figuras de la clase.

## 7. Tablas
En caso de necesitar la inclusión de tablas para organizar información se recomienda el uso de la herramienta del siguiente enlace https://www.tablesgenerator.com/markdown_tables , la cual permite organizar la información dentro de la tabla y genera el código markdown automáticamente:

💡**Ejemplo 3:** 

| **Resultado** | **x = número de intentos hasta primer éxito** |
|---------------|-----------------------------------------------|
|       S       |                       1                       |
|       FS      |                       2                       |
|      FFS      |                       3                       |
|      ...      |                      ...                      |
|    FFFFFFS    |                       7                       |
|      ...      |                      ...                      |

Tabla 1. Tabla de ejemplo

Cada tabla debe llevar la etiqueta que describa su contenido y numeración consecutiva para todas las tablas

## 8. Código
Teniendo en cuenta que el curso requiere del desarrollo de código matlab, c, c++ u otro. Si requiere incluir pequeños segmentos de código en los apuntes hágalos de la siguiente manera:

💡**Ejemplo 4:**
```
var sumar2 = function(numero) {
  return numero + 2;
}
```

## 9. Ejercicios
Deben agregar 2 ejercicios con su respectiva solución, referentes a los temas tratados en cada una de las clases. Para agregar estos, utilice la etiqueta #, es decir como un nuevo título dentro de la clase con la palabra 'Ejercicios'. Cada uno de los ejercicios debe estar numerado y con su respectiva solución inmediatamente despues del enunciado. Antes del subtitulo de cada ejercicio incluya el emoji 📚

## Rúbrica
| 0-1                                                                                   | 1-2                                                                                  | 2-3                                                                                                                                                                               | 3-4                                                                                                                                                                       | 4-5                                                                                                                                                                               |
|---------------------------------------------------------------------------------------|--------------------------------------------------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Presenta menos del 10% de los temas o no presenta por  el medio y formato  solicitado | Presenta menos del 40% de los temas solicitados, y  cumple parcialmente la plantilla | Presenta menos del 60% de los temas solicitados (con descripciones, gráficos tablas, etc), y cumple  parcialmente la plantilla. No presenta la totalidad  de ejercicios resueltos | Presenta menos del 80% de los temas solicitados (con descripciones, gráficos, tablas, etc) y cumple con  la plantilla. No presenta  la totalidad de ejercicios  resueltos | Presenta el 100% de los temas vistos en clase (con descripciones, gráficos, tablas, etc), siguiendo totalmente la plantilla. presenta la  totalidad de los ejercicios solicitados |

## 10. Conclusiones
Agregue unas breves conclusiones sobre los temas trabajados en cada clase, puede ser a modo de resumen de lo trabajado o a indicando lo aprendido en cada clase

## 11. Referencias
Agregue un subtítulo al final donde pueda poner todas las referencias consultadas incluyendo el origen o fuente de los ejercicios planteados. Tambien dentro del texto referencie los textos o artículos consultados y las figuras y tablas dentro de la explicación de las mismas.
