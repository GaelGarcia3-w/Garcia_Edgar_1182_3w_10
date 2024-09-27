# Garcia_Edgar_1182_3w_10
Edgar Gael Garcia Camacho 3-W
def factorial(n):
    if n < 0:
        return "El factorial no está definido para números negativos."
    elif n == 0 or n == 1:
        return 1
    else:
        resultado = 1
        for i in range(2, n + 1):
            resultado *= i
        return resultado

# Solicitar al usuario un número entero
try:
    num = int(input("Introduce un número entero: "))
    resultado = factorial(num)
    print(f"El factorial de {num} es {resultado}.")
except ValueError:
    print("Por favor, introduce un número entero válido.")
