# SomaNumPar
inicio = int(input("Digite o número inicial do intervalo: "))
fim = int(input("Digite o número final do intervalo: "))

somaPares = 0
temPares = False

for numero in range(inicio, fim + 1):
    if numero % 2 == 0:
        somaPares += numero
        temPares = True
        print(numero)
else:
    if not temPares:
        print("Não há números pares no intervalo informado.")

if temPares:
    print(f"A soma dos números pares no intervalo é: {somaPares}")
