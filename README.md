Lectura.py  es el archivo para encontara un block de nota anvos archivos van en una sola carpeta 

---------------------------------------------------------------------------------------------------------

archivo = open("productos.txt", "a")
print("*****Tienda de productos****")
while True:
    nombre = input("Nombre del producto: ")
    if nombre == "":
        break
    precio = float(input(f"Precio unitario de {nombre}:"))
    stock = float(input(f"Stock disponible {nombre}:"))
    archivo.write("\n" + nombre + "\t" + str(precio) + "\t" + str(stock))
   
   
---------------------------------------------------------------------------------------------------------


Lectura.py genera carpeta de blok de nota 


print("\n******Lista de Productos******")
archivo = open("productos.txt", "r")
print(archivo.read())


archivo = open("Datos.txt", "r")


contenido = archivo.read()
print("Contenido del archivo")
print(contenido)

---------------------------------------------------------------------------------------------------------

ejercisio 3.py 

def menu():
    print("1. Ingrese correo ( usuario@dominio.tipo).")
    print("2. Visualizar usuario y tipo")
    print("3. Finalizar")
    
def leercorreo():
    correo = input("Ingrese correo ( usuario@dominio.tipo):")
    return correo

def imprimir(correo):
    pos1 = correo.find("@")
    usuario = correo[0:pos1-1]
    pos2 = correo.find(".")
    tipo = correo[pos2+1: len(correo)]
    print(f"Usuario: {usuario} y el tipo: {tipo}")
    

while True:
    menu()
    op = int(input("Escribir la opcion a seguir: "))
    while op <1 or op >3:
        op = int(input("Opcion no validad. Intente nuevamente: "))
    if op ==1:
        correo = leercorreo()
    elif op ==2:
         print(imprimir(correo))
    elif op ==3:
        print("Gestion finalizada")
        break
    
    



archivo.close()







![image](https://github.com/user-attachments/assets/29b2a62a-eca9-49f3-b30b-88da3db8777d)


