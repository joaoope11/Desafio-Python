# Desafio-Python
Desafio Python para o estágio de férias Navi Capital
## Questão 1:
for n in range (1,5000000):
  if n%2 == 0 and n%49 == 0 and n%37 == 0: 
    print (n)
    
## Questão 2
# Função Fatorial:
def fatorial(x):
    if x == 0 or x == 1:
        return 1 
    else:
        return x * fatorial(x - 1) 
# Montando o vetor:
for i in range(0,9):
  if i%2 == 0 or i == 0:
    vetor[i] = (3 ** i) + (7 *(fatorial(i)))
  else:
    vetor[i] = (2 ** i) + 4 * (np.log(i))
print(vetor)

# Encontrando a posição:
X = vetor.index(max(vetor)) + 1
X

# Encontrando a media:
media = np.average(vetor, axis=0)
Y = media.round(2)
Y

## Questão 3:
# Registrando os nomes e notas dos alunos
a1 = str(input('Digite o nome do primeiro aluno: '))
n1 = float(input('Digite a nota do primeiro aluno: '))
a2 = str(input('Digite o nome do segundo aluno: '))
n2 = float(input('Digite a nota do segundo aluno: '))
a3 = str(input('Digite o nome do terceiro aluno: '))
n3 = float(input('Digite a nota do terceiro aluno: '))
a4 = str(input('Digite o nome do quarto aluno: '))
n4 = float(input('Digite a nota do quarto aluno: '))
a5 = str(input('Digite o nome do quinto aluno '))
n5 = float(input('Digite a nota do quinto aluno '))

# Criando o dicionário
notas_alunos = [(a1,n1),(a2,n2),(a3,n3),(a4,n4),(a5,n5)]
dicionario = dict(notas_alunos)
dicionario

#I mprimindo o aluno com maior nota
X = dicionario[max(dicionario, key=dicionario.get)]
Y = max(dicionario, key=dicionario.get)
print("O aluno com a maior nota foi",Y,", sua nota foi", X)
      
