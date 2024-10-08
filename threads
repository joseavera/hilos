import threading
import time

# Definimos una función que simula la descarga de archivos
def descargar_archivo(nombre_archivo, tiempo_descarga):
    print(f"Iniciando la descarga de {nombre_archivo}...")
    time.sleep(tiempo_descarga)  # Simulamos el tiempo que tarda en descargar
    print(f"Descarga de {nombre_archivo} completada en {tiempo_descarga} segundos.")

# Creación de hilos para simular la descarga de archivos simultáneamente
hilo1 = threading.Thread(target=descargar_archivo, args=("Archivo 1", 3))
hilo2 = threading.Thread(target=descargar_archivo, args=("Archivo 2", 5))

# Iniciar los hilos
hilo1.start()
hilo2.start()


# Esperar a que todos los hilos terminen
hilo1.join()
hilo2.join()


print("Todas las descargas han finalizado.")
