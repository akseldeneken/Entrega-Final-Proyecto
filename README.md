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
**BYAK Clothing Manager** es un programa diseñado para gestionar eficientemente el inventario y los clientes de una tienda de ropa, permitiendo agregar productos y clientes, ordenar el inventario por diferentes criterios y generar reportes de bajo stock.

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
`g++ -std=c++11 mainTienda.cpp -o byak` 
## Ejecución
Ejecuta el siguiente comando en la terminal:
`./byak` 

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

Vectores para inventario:
Mejor caso: O(1) para acceso por índice
Caso promedio:
Acceso: O(1)
Inserción al final: O(1)
Inserción/eliminación en posición intermedia: O(n)
Peor caso: O(n) para inserciones y eliminaciones que requieran reorganizar elementos  
  
Árbol Binario de Búsqueda (BST) para clientes:
Mejor caso (árbol balanceado):
Inserción: O(log n)
Búsqueda: O(log n)
Eliminación: O(log n)
Caso promedio:
Inserción: O(log n)
Búsqueda: O(log n)
Eliminación: O(log n)

Peor caso (árbol completamente desbalanceado):
Inserción: O(n)
Búsqueda: O(n)
Eliminación: O(n)

### 3. **Análisis de Complejidad de Otros Componentes y Complejidad Total**
Función de Importación de Inventario (leerInventarioDesdeArchivo)
Mejor caso: O(n), cuando todos los datos son válidos
Caso promedio: O(n), iterando sobre cada línea del archivo
Peor caso: O(n), con validaciones adicionales
Complejidad espacial: O(m), donde m es el número de productos válidos importados

Función de Generación de Reportes (generaReporteStock)
Mejor caso: O(n), recorriendo una vez el inventario
Caso promedio: O(n), realizando cálculos para cada producto
Peor caso: O(n), con cálculos de porcentajes y escritura en archivo
Complejidad adicional de escritura en archivo: O(1)

Función de Búsqueda de Productos por Precio
Complejidad de ordenamiento previo: O(n log n)
Complejidad de búsqueda binaria: O(log n)
Complejidad total: O(n log n), dominada por el ordenamiento

Operaciones de Menú Principal
Mostrar Menú: O(1)
Lectura de Opción: O(1)
Ejecución de Opción: Varía según la operación específica

Ordenamiento: O(n log n)
Búsqueda: O(log n)
Inserción: O(1) o O(log n) dependiendo de la estructura

Complejidad Espacial General
Uso de vectores para inventario: O(n)
Árbol Binario de Búsqueda para clientes: O(m), donde m es número de clientes
Espacio adicional para operaciones temporales: O(log n) o O(n) dependiendo de la operación

Ya que el programa efectúa una secuencia de operaciones de inserción, eliminación y búsqueda, la complejidad final del programa sería: (O(n))

## SICT0302: Toma decisiones
#### Selección del Algoritmo de Ordenamiento
Para el ordenamiento del inventario, se utilizó Merge Sort debido a sus características específicas:
Complejidad Temporal Consistente: O(n log n) en todos los casos
Estabilidad: Mantiene el orden relativo de elementos con valores iguales
Rendimiento Predecible: No depende de la disposición inicial de los datos
Eficiencia para Grandes Volúmenes: Ideal para inventarios extensos

Ventajas sobre otros algoritmos:

Más estable que Quick Sort
Mejor rendimiento que Bubble Sort o Insertion Sort para grandes conjuntos de datos
Divide el problema recursivamente, lo que facilita su implementación y comprensión

## Selección de Estructuras de Datos
Vectores para Inventario
Razones para su elección:
Acceso directo por índice en O(1)
Memoria contigua que mejora el rendimiento de acceso
Flexibilidad para modificar elementos
Compatibilidad con algoritmos de ordenamiento como Merge Sort

Árbol Binario de Búsqueda (BST) para Clientes
Consideraciones:
Permite búsquedas ordenadas
Inserción y eliminación relativamente eficientes
Limitación Importante: No garantiza balanceo automático

Recomendación de Mejora: Para operaciones consistentes O(log n), considerar implementar un Árbol AVL o Árbol Rojo-Negro que mantengan el balance automáticamente.
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





