# Proyecto-final-Python-basico
Proyecto final curso python nivel basico Platzi
#proyecto final:  Hacer un programa que simule un cajero automatico
#Nombre: Wilson Lancheros Cárdenas

saldo = 500000

print("t\.:MENU:.")
print("1. Ingresar dinero en la cuenta")
print("2. Retirar dinero de la cuenta")
print("3. Mostrar dinero disponible")
print("4. Salir")
opcion = int(input("Digite una opcion de menu: "))

print()

if opcion==1:
   extra = float(input("cuanto dinero desea ingresar -> "))
   saldo = saldo + extra
   print(f"dinero en la cuenta : {saldo}")
elif opcion==2:
   retirar = float(input("cuanto dinero desea retirar ->"))
   if retirar>=saldo:
      print("No tiene esa cantidad de dinero")
   else:
      saldo = saldo - retirar
      print(f"dinero en la cuenta : {saldo}")
elif opcion==3:
   print(f"dinero en la cuenta : {saldo}")
elif opcion==4:
   print("Gracias por utilizar nuestros servicios")
else:
   print("error, se equivoco de opcion de menu")
