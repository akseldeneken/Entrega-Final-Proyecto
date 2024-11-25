# Entrega-Final-Proyecto
# Sistema de Gestión de Tienda de Ropa "BYAK CLOTHING"
Este programa permite gestionar el inventario de una tienda de ropa, proporcionando funcionalidades para ordenar productos, gestionar clientes, y generar reportes. El sistema utiliza diferentes estructuras de datos y algoritmos para manejar eficientemente tanto el inventario como la base de datos de clientes.

## Descripción Avance 1
En el primer avance del proyecto se realizó un prototipo de un sistema básico de gestión de inventario para una tienda de ropa llamada "BYAK CLOTHING". El sistema incluía una estructura de dos clases principales: Producto para manejar la información básica de cada artículo (precio, nombre, stock) y Tienda para gestionar el inventario. Las funcionalidades iniciales permitían visualizar el inventario, ordenar productos por diferentes criterios utilizando MergeSort (precio, nombre, stock), realizar búsquedas binarias por precio y agregar nuevos productos al inventario. La interfaz de usuario consistía en un menú simple con 6 opciones básicas de gestión.

## Descripción Avance 2
En el segundo avance se expandieron significativamente las capacidades del sistema añadiendo un módulo completo de gestión de clientes mediante un árbol binario de búsqueda (BST), que permite agregar, buscar por nombre o ID, y eliminar y listar clientes de manera ordenada. Se agregaron nuevas funcionalidades críticas como la capacidad de importar productos desde archivos externos. 

# Cambios Sobre el primer avance
Cambio 1: Nuevas funcionalidades: Gestión de clientes usando un árbol binario de búsqueda (BST).
Cambio 2: Menú ampliado: Se agregan opciones para manejar clientes (agregar, buscar, eliminar, listar).
Cambio 3: Manejo de archivos: Capacidad de leer inventarios desde archivos externos.
Cambio 4: Separación de funcionalidades en diferentes archivos (Clientes.h, productos.h).

## Descripción Último Avance
Este último avance incluye mejoras significativas en la gestión del sistema, destacando la implementación de reportes personalizados para productos con bajo stock, donde se detalla el valor del inventario en riesgo de quedarse "sold out", las unidades faltantes y el porcentaje de productos afectados, con opción de exportarlos a archivos. También se optimiza la presentación del inventario mediante tablas alineadas y encabezados claros, además de perfeccionar la búsqueda binaria para números flotantes con tolerancia. Se agregan validaciones robustas para la importación de datos desde archivos externos, asegurando que solo se procesen valores válidos, y se amplía el menú con opciones como generación de reportes, mientras se mantiene el manejo eficiente de clientes y productos mediante estructuras como BST y vectores.

# Cambios Sobre el segundo avance
Cambio 1: Reportes personalizados: Generación de reportes de bajo stock con detalles como unidades necesarias y valor en riesgo.
Cambio 2: Mejoras visuales: Presentación del inventario con tablas formateadas y encabezados claros.
Cambio 3: Validación de datos: Mayor control en la importación de inventarios desde archivos, ignorando entradas inválidas.
Cambio 4: Optimización: Ajustes en la búsqueda binaria para trabajar con flotantes y tolerancia.
Cambio 5: Ampliación del menú: Nuevas opciones, como generar reportes y un manejo más detallado del inventario.

## Descripción del proyecto
**BYAK Clothing Management** es un programa diseñado para gestionar eficientemente el inventario y los clientes de una tienda de ropa, permitiendo agregar productos y clientes, ordenar el inventario por diferentes criterios y generar reportes de bajo stock.

Gestión de Inventario: Los productos se organizan en un vector y pueden ordenarse según atributos como precio, nombre o cantidad en stock mediante el algoritmo Merge Sort. Además, incluye funcionalidades de búsqueda binaria para localizar productos por precio y la capacidad de importar inventarios desde archivos externos, validando los datos ingresados.

Gestión de Clientes: Los clientes se manejan con un árbol binario de búsqueda (BST), permitiendo agregar, buscar, eliminar y listar clientes en orden alfabético. Esto asegura un manejo estructurado y eficiente de la base de datos de clientes.

Reportes Personalizados: El programa puede generar reportes detallados sobre productos con bajo stock, indicando unidades necesarias, valor en riesgo y porcentaje de inventario afectado, exportándolos a archivos externos para análisis adicional.

Presentación y Validación: El sistema incluye una interfaz de consola con tablas formateadas para visualizar el inventario de forma clara y valida los datos de entrada para evitar errores en la gestión.

## Funcionamiento
Al iniciar el programa se mostrará el siguiente menú de opciones: 
1. Ordenar Productos Por Precio
2. Ordenar Productos Por Nombre
3. Ordenar Productos Por Cantidad En Stock
4. Buscar Producto por Precio
5. Añadir Producto
6. Ordenar Clientes Por Nombre
7. Buscar Cliente Por Nombre
8. Buscar Cliente Por ID
9. Añadir Cliente
10. Eliminar Cliente
11. Agregar Productos Desde Archivo Externo
12. Generar reporte de bajo Stock
13. Salir

Se destacan las siguientes funcionalidades principales:
- Ordenamiento de productos por precio, nombre y stock
- Gestión de clientes mediante un árbol binario de búsqueda (BST)
- Búsqueda de productos por precio
- Generación de reportes de inventario bajo stock
- Importación de productos desde archivos externos

## Compilación
Ejecuta el siguiente comando en la terminal:
`g++ -std=c++11 mainTienda.cpp` 
`./a out` 

## Clases Principales
En el proyecto existen las siguientes clases:
1. **Producto**: Representa un artículo de ropa con atributos como precio, nombre y stock
2. **Cliente**: Representa a un cliente de la tienda y se maneja la información de los mismos, tienen atributos como ID y Nombre
3. **Tienda**: Gestiona todas las operaciones relacionadas con el inventario
4. **BSTCliente**: Implementa el árbol binario de búsqueda para la gestión de clientes
   
## Descripción de las entradas del proyecto
El sistema recibe como entradas los siguientes datos sobre los productos y los clientes:
- **Productos**: precio (float), nombre (string), stock (int)
- **Clientes**: nombre (string), ID (int)
- **Archivos de entrada**: formato de texto con datos de productos
- **Parámetros de reportes**: límite de stock, nombre del archivo

## Descripción de las salidas del proyecto
Las salidas del proyecto incluyen:
- Listados ordenados de productos
- Resultados de búsquedas de productos y clientes
- Reportes de inventario bajo stock en archivos de texto
- Confirmaciones de operaciones realizadas

## Consideraciones
- El sistema maneja un inventario predeterminado inicial
- Los archivos de entrada deben seguir el formato especificado
- Los reportes se generan en archivos de texto separados
- El sistema valida las entradas para prevenir errores

## Casos de Uso Típicos
El sistema demuestra su utilidad en las siguientes situaciones que una tienda podría enfrentar:
1. Búsqueda de productos por rango de precio
2. Gestión de inventario y alertas de stock bajo
3. Mantenimiento de base de datos de clientes
4. Generación de reportes de inventario

### Desarrollo de Competencias
## SICT0301: Evalúa los componentes
Se implementaron diferentes estructuras de datos y algoritmos, evaluando su eficiencia y seleccionando los más apropiados para cada operación:

## Análisis de complejidad para los algoritmos de ordenamiento usados en el programa:
Merge Sort: Este algoritmo tiene una complejidad temporal de O(nlogn), ya que divide el vector en mitades de forma recursiva (O(logn)) y las combina ordenadamente en O(n). Se eligió debido a que este es adecuado para listas grandes por su eficiencia y estabilidad.

Búsqueda Binaria: Tiene una complejidad de O(logn), ya que reduce la búsqueda a la mitad en cada iteración. Se eligió debido a que asegura una localización rápida en vectores previamente ordenados.

### 2. **Análisis de Complejidad de Estructuras de Datos**
Vectores para inventario: Los vectores ofrecen acceso O(1) a elementos por índice y son óptimos para ordenamientos debido a su disposición contigua en memoria. Operaciones como inserción al final tienen complejidad O(1), pero agregar elementos en posiciones intermedias o eliminarlos es O(n).

Árbol Binario de Búsqueda (BST) para clientes: La inserción, búsqueda y eliminación tienen una complejidad promedio de O(logn), aunque en el peor caso, si el árbol está desbalanceado, puede llegar a O(n). Esto es mitigado con la implementación cuidadosa de las operaciones.

### 3. **Análisis de Complejidad de Otros Componentes y Complejidad Total**
El programa combina los algoritmos de ordenamiento y búsqueda con estructuras eficientes, logrando una complejidad general de O(nlogn) para operaciones de inventario (ordenamiento y búsqueda). Operaciones adicionales, como el manejo del BST para clientes, no impactan significativamente el rendimiento global gracias a su promedio de complejidad de O(logn).

## SICT0302: Toma decisiones
#### Selección del Algoritmo de Ordenamiento
Dado que la gestión eficiente del inventario y la experiencia del cliente son prioridades para BYAK Clothing, se seleccionaron algoritmos y estructuras que optimizan el rendimiento en contextos dinámicos. La solución aborda tanto el manejo del inventario como la gestión de clientes, adaptándose a las necesidades específicas de cada caso.

Eficiencia en Ordenamiento:
Se utilizó Merge Sort para ordenar el inventario por precio, nombre o stock, ya que garantiza una complejidad de O(nlogn) en el peor caso, manteniendo estabilidad y eficacia incluso para grandes volúmenes de datos. Esto asegura una organización clara del inventario para consultas rápidas y precisas. Aunque algoritmos como Quick Sort pueden ser más rápidos en promedio, Merge Sort es más consistente y no depende de la disposición inicial de los datos.

Gestión Dinámica de Clientes:
Para manejar una base de datos de clientes que crece y cambia constantemente, se implementó un árbol binario de búsqueda (BST). Este permite buscar, agregar y eliminar clientes con una complejidad promedio de O(logn), manteniendo el sistema eficiente incluso con muchas operaciones. A diferencia de listas enlazadas o vectores, el BST asegura un acceso ordenado y tiempos consistentes para operaciones clave.

### Selección de la Estructura de Datos
Vectores para Inventario:
Los vectores permiten aprovechar la continuidad en memoria para ordenamientos rápidos con Merge Sort y búsquedas eficientes con algoritmos como la búsqueda binaria. Ofrecen flexibilidad para modificar el inventario mediante inserciones y eliminaciones, equilibrando simplicidad y rendimiento.

Árbol Binario de Búsqueda para Clientes:
La estructura garantiza un orden dinámico sin la necesidad de reordenar explícitamente tras cada inserción o eliminación. Facilita listados ordenados de clientes y búsquedas rápidas tanto por nombre como por ID, siendo ideal para bases de datos en crecimiento.

Merge Sort para Ordenamiento:
Este algoritmo proporciona un balance entre rendimiento y estabilidad, esencial para manejar atributos como precios o nombres. Permite ordenar el inventario completo en tiempo eficiente, mejorando la experiencia del usuario al consultar productos organizados.

Búsqueda Binaria para Consultas:
Con una complejidad de O(logn), es ideal para localizar productos rápidamente en un inventario previamente ordenado. Minimiza el tiempo de búsqueda, clave para una gestión de inventario eficiente en tiempo real.

Adaptabilidad a Cambios Dinámicos
El diseño del proyecto permite integrar nuevos productos y clientes sin comprometer el rendimiento. Las operaciones de inserción y eliminación en el BST garantizan un manejo fluido de clientes, mientras que el uso de vectores facilita la integración de datos de inventario desde archivos externos. Esto asegura que el sistema pueda adaptarse a un flujo constante de cambios en tiempo real, sin necesidad de reorganizaciones completas tras cada modificación.

## SICT0303: Implementa acciones científicas
Considero que aprendí a aplicar correctamente los mecanismos de consulta, lectura y escritura de información para las estructuras de datos vistas en clase, seleccionando aquellas que mejor se adaptaran a los requerimientos del proyecto. Reflexioné sobre el uso real del código en la gestión de inventarios y clientes, priorizando la eficiencia y funcionalidad en cada componente poniendome en el lugar de el dueño d euna tienda de ropa. Me enfoqué en implementar estructuras y algoritmos que no solo fueran eficientes, sino también adaptables, buscando optimizar el manejo del inventario y la experiencia de consulta para los usuarios.

Vease:

Archivo (GestionTienda.h): Función mergeSort (líneas 102-143) para el ordenamiento eficiente del inventario según diferentes atributos.
Archivo (Clientes.h): Funciones insertar y buscar (líneas 73-97) para el manejo dinámico de clientes con un BST.
Archivo (main.cpp): Función mostrarInventario (líneas 29-64) para la presentación clara y ordenada del inventario.

Logré implementar correctamente la lectura de datos desde archivos, utilizando validaciones para prevenir errores como valores inválidos o formatos incorrectos, asegurando que solo se cargaran datos confiables al sistema. 

Vease:

Archivo (GestionTienda.h): Función leerInventarioDesdeArchivo (líneas 145-175) para importar productos desde archivos externos con validaciones detalladas.

Asimismo, comprendí y apliqué los fundamentos para escribir archivos de manera efectiva. Esto incluyó la generación de reportes personalizados que mencionan información crítica para los usuarios, como productos con bajo stock y análisis del impacto en el inventario. 

Vease:

Archivo (GestionTienda.h): Función generaReporteStock (líneas 177-224) para la creación de reportes detallados y exportación a archivos externos.

En general, este proyecto fue una gran oportunidad para aprender y consolidar conocimientos, pero quiero mencionar que enfrenté varios desafíos desde el inicio. Después de tomar clase con Peter, mi progreso en programación se vio muy afectado, lo que me llevó a llegar a esta materia con un nivel casi nulo en programación. Esto complicó tanto las actividades como la realización del proyecto. Sin embargo, logré superar esas dificultades y crear un proyecto sólido y funcional, lo cual considero un gran logro. Durante el proceso, logré retomar parte del conocimiento y habilidades que tenía antes, y redescubrí lo mucho que disfruto programar, lo que hizo que el proceso, aunque complicado, también fuera gratificante.

Para completar el proyecto, recurrí a varias fuentes de apoyo, incluyendo videos en YouTube, herramientas como ChatGPT y Claude, además de la orientación en clase. Estas herramientas complementaron mi aprendizaje y me ayudaron a entender conceptos que en un principio parecían inalcanzables. Ahora tengo claro que debo seguir practicando por mi cuenta para mejorar mi nivel como programador y alcanzar el nivel que quiero.

Gracias por todo, profesor. Realmente aprendí mucho en su clase. Si en algún momento parecía desinteresado o me salía, era porque me sentía perdido, pero siempre intenté esforzarme. Creo que este proyecto refleja todo el conocimiento que he acumulado hasta ahora, y me siento orgulloso del resultado. 





