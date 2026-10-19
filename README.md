🖥️ Simulador de Procesos en Python
Un simulador de planificación de procesos y gestión de CPU desarrollado en Python, diseñado con fines educativos 
para comprender el funcionamiento básico de los Sistemas Operativos.

🚀 Características Principales
Carga Interactiva de Procesos: Permite registrar de 1 a 4 procesos con tiempos de llegada y ráfagas de CPU configurables en unidades de tiempo.
Validación de Entradas: Control robusto de errores para asegurar que los ingresos del usuario sean numéricos, válidos y múltiplos requeridos.
Algoritmos de Planificación Soportados:
FIFO (First In, First Out): Planificación no expropiativa basada en el orden de llegada a la cola de listos.
SRTF (Shortest Remaining Time First): Planificación expropiativa (con desalojo) basada en el tiempo restante de la ráfaga de CPU más corta.
Diagrama de Tiempo / Proceso: Generación automática de una representación gráfica en consola que detalla el estado del sistema operativo, 
colas de listos, bloqueados por E/S y el uso del procesador por cada unidad de tiempo.

📋 Requisitos del Sistema
Python 3.x instalado en tu equipo.

🎮 Cómo Ejecutar el Programa
Clona el repositorio o descarga el archivo fuente con el código del simulador (por ejemplo, simulador.py).
Abre una terminal o línea de comandos en la carpeta del archivo.
Ejecuta el script con el siguiente comando:python simulador.py
Sigue las instrucciones del menú interactivo en pantalla:
  1. Cargar procesos: Ingresa la cantidad de procesos y sus respectivos tiempos/ráfagas.
   2. Mostrar procesos: Visualiza los datos actuales guardados en memoria.
   3. 3. Simular ejecución: Selecciona el algoritmo (FIFO o SRTF) para ver la ejecución paso a paso y el diagrama final.
  4. Salir: Cierra la aplicación.

🛠️ Estructura del Código
leer_entero(mensaje): Valida la entrada por teclado para prevenir excepciones por caracteres no numéricos.
cargar_procesos(): Solicita y valida los parámetros de los procesos.
mostrar_procesos(): Muestra los procesos ingresados por pantalla.
fifo(procesos): Simula la política de despacho secuencial sin desalojo.
srtf(procesos): Simula la política expropiativa priorizando el proceso con menor tiempo de ráfaga pendiente.
imprimir_diagrama(...): Dibuja por consola la grilla temporal de estados y acciones del S.O.
