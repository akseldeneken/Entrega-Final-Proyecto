# Entrega-Final-Proyecto
# Sistema de Gestión de Tienda de Ropa "BYAK CLOTHING"

## Descripción del Proyecto
Este programa permite gestionar el inventario de una tienda de ropa, proporcionando funcionalidades para ordenar productos, gestionar clientes, y generar reportes. El sistema utiliza diferentes estructuras de datos y algoritmos para manejar eficientemente tanto el inventario como la base de datos de clientes.

## Descripción Avance 1

## Descripción Avance 1

# Cambios Sobre el primer avance

# Cambios Sobre el primer avance

# Descripción del proyecto

# Funcionamiento

### Compilación
`g++ -std=c++11 mainTienda.cpp` 
`./a.out` 

## Descripción de las entradas del proyecto

## Descripción de las salidas del proyecto

### Desarrollo de Competencias

## SICT0301: Evalúa los componentes

### 2. **Análisis de Complejidad de Estructuras de Datos**

### 3. **Análisis de Complejidad de Otros Componentes**

### 4. **Complejidad Final del Programa**

## SICT0302: Toma decisiones

#### Selección del Algoritmo de Ordenamiento

#### Selección de la Estructura de Datos

## SICT0303: Implementa acciones científicas


### Funcionalidades Principales
- Ordenamiento de productos por precio, nombre y stock
- Gestión de clientes mediante un árbol binario de búsqueda (BST)
- Búsqueda de productos por precio
- Generación de reportes de inventario bajo stock
- Importación de productos desde archivos externos

## Estructura del Proyecto

### Clases Principales
1. **Producto**: Representa un artículo de ropa con atributos como precio, nombre y stock
2. **Cliente**: Maneja la información de los clientes
3. **Tienda**: Gestiona todas las operaciones relacionadas con el inventario
4. **BSTCliente**: Implementa el árbol binario de búsqueda para la gestión de clientes

### Algoritmos Implementados
1. **MergeSort**: Utilizado para ordenar productos por diferentes criterios
   - Complejidad: O(n log n) en todos los casos
2. **Búsqueda Binaria**: Para encontrar productos por precio
   - Complejidad: O(log n) después del ordenamiento
3. **BST**: Para gestionar clientes
   - Inserción: O(log n) en caso promedio
   - Búsqueda: O(log n) en caso promedio
   - Eliminación: O(log n) en caso promedio

## Análisis de Complejidad

### Operaciones sobre Productos
- **Ordenamiento (MergeSort)**:
  - Mejor caso: O(n log n)
  - Caso promedio: O(n log n)
  - Peor caso: O(n log n)

### Operaciones sobre Clientes (BST)
- **Inserción**:
  - Mejor caso: O(1) cuando la raíz está vacía
  - Caso promedio: O(log n) en un árbol balanceado
  - Peor caso: O(n) en un árbol degenerado

- **Búsqueda**:
  - Mejor caso: O(1) cuando el elemento está en la raíz
  - Caso promedio: O(log n)
  - Peor caso: O(n)

## Instrucciones de Uso



### Menú de Opciones
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

## Entradas del Sistema
- **Productos**: precio (float), nombre (string), stock (int)
- **Clientes**: nombre (string), ID (int)
- **Archivos de entrada**: formato de texto con datos de productos
- **Parámetros de reportes**: límite de stock, nombre del archivo

## Salidas del Sistema
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
1. Búsqueda de productos por rango de precio
2. Gestión de inventario y alertas de stock bajo
3. Mantenimiento de base de datos de clientes
4. Generación de reportes de inventario

## Desarrollo de Competencias

### SICT0301: Evalúa los componentes
Se implementaron diferentes estructuras de datos y algoritmos, evaluando su eficiencia y seleccionando los más apropiados para cada operación:
- MergeSort para ordenamiento flexible de productos
- BST para gestión eficiente de clientes
- Búsqueda binaria para localización rápida de productos

### SICT0302: Toma decisiones
La selección de estructuras de datos y algoritmos se basó en:
- Necesidad de ordenamiento eficiente para múltiples criterios
- Requisito de búsqueda rápida tanto en productos como clientes
- Manejo dinámico de inventario y base de datos de clientes

### SICT0303: Implementa acciones científicas
El proyecto demuestra la aplicación práctica de conceptos de ciencias computacionales:
- Implementación de estructuras de datos complejas
- Uso de algoritmos de ordenamiento y búsqueda
- Manejo de archivos para persistencia de datos
