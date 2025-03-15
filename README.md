# Convers-o-de-Temperatura-em-Python
#Linhas de código em Python para conversão de temperatura
def celsius_to_fahrenheit(c):
    return (c * 1.8) + 32

def celsius_to_kelvin(c):
    return c + 273.15

def fahrenheit_to_celsius(f):
    return (f - 32) / 1.8

def fahrenheit_to_kelvin(f):
    return (f - 32) * 5/9 + 273.15

def kelvin_to_celsius(k):
    return k - 273.15

def kelvin_to_fahrenheit(k):
    return (k - 273.15) * 1.8 + 32

def main():
    print("Conversor de Temperatura")
    print("1 - Celsius para Fahrenheit")
    print("2 - Celsius para Kelvin")
    print("3 - Fahrenheit para Celsius")
    print("4 - Fahrenheit para Kelvin")
    print("5 - Kelvin para Celsius")
    print("6 - Kelvin para Fahrenheit")
    
    opcao = int(input("Escolha a conversão desejada (1-6): "))
    valor = float(input("Digite o valor da temperatura: "))
    
    if opcao == 1:
        print(f"Resultado: {celsius_to_fahrenheit(valor):.2f} °F")
    elif opcao == 2:
        print(f"Resultado: {celsius_to_kelvin(valor):.2f} K")
    elif opcao == 3:
        print(f"Resultado: {fahrenheit_to_celsius(valor):.2f} °C")
    elif opcao == 4:
        print(f"Resultado: {fahrenheit_to_kelvin(valor):.2f} K")
    elif opcao == 5:
        print(f"Resultado: {kelvin_to_celsius(valor):.2f} °C")
    elif opcao == 6:
        print(f"Resultado: {kelvin_to_fahrenheit(valor):.2f} °F")
    else:
        print("Opção inválida! Escolha um número entre 1 e 6.")

if __name__ == "__main__":
    main()
