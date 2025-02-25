Lectura.py  es el archivo para encontara el archivo .

archivo = open("productos.txt", "a")
print("*****Tienda de productos****")
while True:
    nombre = input("Nombre del producto: ")
    if nombre == "":
        break
    precio = float(input(f"Precio unitario de {nombre}:"))
    stock = float(input(f"Stock disponible {nombre}:"))
    archivo.write("\n" + nombre + "\t" + str(precio) + "\t" + str(stock))
   
   


Lectura.py genera carpeta de blok de nota 


print("\n******Lista de Productos******")
archivo = open("productos.txt", "r")
print(archivo.read())


archivo = open("Datos.txt", "r")


contenido = archivo.read()
print("Contenido del archivo")
print(contenido)



archivo.close()


