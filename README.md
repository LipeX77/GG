soma_homens = 0
soma_mulheres = 0
cont_homens = 0
cont_mulheres = 0
soma_total = 0

for i in range(10):
    idade = int(input("Digite a idade: "))
    sexo = input("Digite o sexo (M/F): ")

    soma_total += idade

    if sexo == 'M':
        soma_homens += idade
        cont_homens += 1
    elif sexo == 'F':
        soma_mulheres += idade
        cont_mulheres += 1
if cont_homens > 0:
    media_homens = soma_homens / cont_homens
else:
    media_homens = 0

if cont_mulheres > 0:
    media_mulheres = soma_mulheres / cont_mulheres
else:
    media_mulheres = 0

media_total = soma_total / 10
print("Idade média das mulheres:", media_mulheres)
print("Idade média dos homens:", media_homens)
print("Idade média do grupo:", media_total)
