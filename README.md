import math

vet_nome_item = []
vet_preco_item = []
count = 0
numpedidos = float(input("Digite o Numero de itens: "))
total = 0

while (count < numpedidos):
    nome_item = input(f"Digite o nome do item {count+1}: ")
    preco_item = float(input(f"Digite o preço do item {count+1}: "))
    total = total + preco_item
    vet_nome_item.append(nome_item)
    vet_preco_item.append(preco_item)
    count = count + 1

print(total)
C_cadastrado = input("Digite s caso clente cadastrado e n caso não: ")

if (C_cadastrado == "s"):
    total = total * 0.9
    print(f"O valor total é de {total:.2f}")
else:
    print(f"O valor total é de {total:.2f}")

countl = 0
print("A lista completa de items é")
while (countl< numpedidos):
    print(f"O item {countl+1} é {vet_nome_item[countl]} e tem preço {vet_preco_item[countl]:.2f}")
    countl = countl + 1
