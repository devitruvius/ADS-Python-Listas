# Estruturas de Listas em Python

Este repositório apresenta uma série de exemplos de código em Python que demonstram a aplicação das estruturas de listas. Os códigos foram elaborados como parte das atividades da disciplina de Fundamentos de Algoritmo do curso de Análise e Desenvolvimento de Sistemas (ADS) pela Universidade Federal do Cariri (UFCA). O principal objetivo dessas atividades é proporcionar uma prática sólida e consolidar os conceitos essenciais relacionados às estruturas de coleções em Python, buscando a compreensão aprofundada e o aprimoramento das habilidades de programação.

## Estrutura do Repositório

A estrutura do repositório foi organizada para proporcionar uma experiência de navegação eficiente e facilitar a revisão dos códigos. Cada bloco de atividade está representada por um tópico, dentro do qual você encontrará os códigos referentes às atividades desenvolvidas.

## Atividades

1. **Faça um Programa que leia uma lista de 5 números inteiros e mostre-os.**

   ```python
   # Algoritmo Coletor de Cinco Números
   # Declaração de Variáveis
   
   # Inicializando uma lista vazia para armazenar os números
   numeros = []
   
   # Loop para ler 5 números inteiros
   for i in range(5):
       numero = int(input(f"Digite o {i+1}º número inteiro: "))
       numeros.append(numero)
   
   # Mostrando os números
   print("Números digitados:")
   for numero in numeros:
       print(numero)
   ```
<hr>

2. **Faça um Programa que leia uma lista de 10 números reais e mostre-os na ordem inversa.**
 
   ```python
   # Reversor de Números Reais
   # Declaração de Variáveis
   
   # Inicializando uma lista vazia para armazenar os números
   numeros_reais = []
   
   # Loop para ler 10 números reais
   for i in range(10):
     numero_real = float(input(f"Digite o {i+1}º número real: "))
     numeros_reais.append(numero_real)
   
   # Mostrando os números
   print("\nNúmeros digitados:")
   for numero_real in reversed(numeros_reais):
     print(numero_real)
   ```
<hr> 

3. **Faça um Programa que leia 4 notas, mostre as notas e a média na tela.**

   ```python
   # Calculadora de Média de Notas
   # Declaração de Variáveis
   
   # Inicializando uma lista vazia para armazenar as notas
   notas = []
   
   # Loop para ler 4 notas
   for i in range(4):
       nota = float(input(f"Digite a {i+1}ª nota: "))
       notas.append(nota)
   
   # Mostrando as notas
   print("\nNotas digitadas:")
   for nota in notas:
       print(nota)
   
   # Calculando a média
   media = sum(notas) / len(notas)
   
   # Mostrando a média na tela
   print(f"\nMédia das notas: {media}")
   ```
<hr>
 
4. **Faça um Programa que leia uma lista de 10 caracteres, e diga quantas consoantes foram lidas. Imprima as consoantes.**

   ```python
   # Identificador e Contador de Consoantes
   # Declaração de Variáveis
   
   # Inicializando uma lista vazia para armazenar os caracteres
   caracteres = []
   
   # Lista para armazenar as consoantes
   consoantes = []
   
   # Loop para ler 10 caracteres
   for i in range(10):
       caractere = input(f"Digite o {i+1}º caractere: ")
       caracteres.append(caractere)
   
   # Verificando e contando as consoantes
   for caractere in caracteres:
       if caractere.isalpha() and caractere.lower() not in ['a', 'e', 'i', 'o', 'u']:
           consoantes.append(caractere)
   
   # Imprimindo as consoantes e a quantidade
   print("\nConsoantes digitadas:")
   for consoante in consoantes:
       print(consoante)
   
   print("\nQuantidade de consoantes:", len(consoantes))
   ```
<hr>

5. **Faça um Programa que leia 20 números inteiros e armazene-os numa lista. Armazene os números pares na lista PAR e os números IMPARES na lista impar. Imprima as três listas.**

   ```python
   # Classificador de Números Inteiros
   # Declaração de Variáveis
   
   # Inicializando uma lista vazia para armazenar os números inteiros
   numeros = []
   
   # Listas para armazenar números pares e ímpares
   pares = []
   impares = []
   
   # Loop para ler 20 números inteiros
   for i in range(20):
       numero = int(input(f"Digite o {i+1}º número inteiro: "))
       numeros.append(numero)
   
   # Separando os números pares dos ímpares
   for numero in numeros:
       if numero % 2 == 0:
           pares.append(numero)
       else:
           impares.append(numero)
   
   # Imprimindo as três listas
   print("\nNúmeros digitados:", numeros)
   print("\nNúmeros pares:", pares)
   print("\nNúmeros ímpares:", impares)
   ```
<hr>

6. **Faça um Programa que peça as quatro notas de 10 alunos, calcule e armazene numa lista a média de cada aluno, imprima o número de alunos com média maior ou igual a 7.0.**

   ```python
   # Calculador de Médias e Contador de Alunos Aprovados
   # Declaração de Variáveis
   
   # Lista para armazenar as médias dos alunos
   medias_alunos = []
   
   # Contador para o número de alunos com média maior ou igual a 7.0
   alunos_aprovados = 0
   
   # Loop para iterar sobre os 10 alunos
   for i in range(10):
       # Lista para armazenar as notas do aluno
       notas_aluno = []
       print(f"Aluno {i+1}:")
       # Loop para ler as quatro notas do aluno
       for j in range(4):
           nota = float(input(f"Digite a {j+1}ª nota: "))
           notas_aluno.append(nota)
       
       # Calculando a média do aluno
       media_aluno = sum(notas_aluno) / len(notas_aluno)
       medias_alunos.append(media_aluno)
   
       # Verificando se a média do aluno é maior ou igual a 7.0
       if media_aluno >= 7.0:
           alunos_aprovados += 1
   
   # Imprimindo o número de alunos aprovados
   print("\nNúmero de alunos com média maior ou igual a 7.0:", alunos_aprovados)
   ```
<hr>

7. **Faça um Programa que leia uma lista de 5 números inteiros, mostre a soma, a multiplicação e os números.**

   ```python
   # Calculadora de Soma e Multiplicação de Números Inteiros
   # Declaração de Variáveis
   
   # Inicializando uma lista para armazenar os números inteiros
   numeros_inteiros = []
   
   # Loop para iterar sobre os números inteiros digitados pelo usuário
   for i in range(5):
     numero_inteiro = int(input(f'Digite o {i+1}º número inteiro: '))
     numeros_inteiros.append(numero_inteiro)
   
   # Calculando as operações matemáticas
   soma = sum(numeros_inteiros)
   multiplicacao = 1
   for numero_inteiro in numeros_inteiros:
     multiplicacao *= numero_inteiro
   
   # Mostrando os resultados
   print(f"\nNúmeros digitados: {numeros_inteiros}")
   print("Soma dos números:", soma)
   print("Multiplicação dos números:", multiplicacao)
   ```
<hr>

8. **Faça um Programa que peça a idade e a altura de 5 pessoas, armazene cada informação na sua respectiva lista. Imprima a idade e a altura na ordem inversa a ordem lida.**
    
   ```python
   # Reversor de Idades e Alturas
   # Declaração de Variáveis
   
   # Inicializando uma lista para armazenar as idades
   idades = []
   
   # Inicializando uma lista para armazenar as alturas
   alturas = []
   
   # Loop para ler idade e altura
   for i in range(5):
     idade = int(input(f'Digite a idade da {i+1}º pessoa: '))
     idades.append(idade)
     altura = float(input(f'Digite a altura da {i+1}º pessoa: '))
     alturas.append(altura)
   
   # Imprimindo as idades e alturas na ordem inversa
   print("\nIdades na ordem inversa:")
   for idade in reversed(idades):
       print(idade)
   
   print("\nAlturas na ordem inversa:")
   for altura in reversed(alturas):
       print(altura)
   ```
<hr>

9. **Faça um Programa que leia uma lista A com 10 números inteiros, calcule e mostre a soma dos quadrados dos elementos da lista.**

   ```python
   # Calculadora de Soma de Quadrados
   # Declaração de Variáveis
   
   # Inicializando a lista vazia para armazenar os números inteiros
   lista = []
   
   # Loop para ler 10 números inteiros
   for i in range(10):
       numero = int(input(f"Digite o {i+1}º número inteiro: "))
       lista.append(numero)
   
   # Calculando a soma dos quadrados dos elementos da lista
   soma_quadrados = sum(numero ** 2 for numero in lista)
   
   # Mostrando o resultado
   print("\nA soma dos quadrados dos elementos da lista é:", soma_quadrados)
   ```
<br>

10. **Faça um Programa que leia duas listas com 10 elementos cada. Gere uma terceira lista de 20 elementos, cujos valores deverão ser compostos pelos elementos intercalados dos duas outras listas.**

    ```python
    # Intercalador de Listas 
    # Declaração de Variáveis
    
    # Inicializando duas listas vazias para armazenar os elementos das listas
    lista1 = []
    lista2 = []
    
    # Lendo os elementos da primeira lista
    print("Digite os elementos da primeira lista:")
    for i in range(10):
        elemento = input(f"Digite o {i+1}º elemento: ")
        lista1.append(elemento)
    
    # Lendo os elementos da segunda lista
    print("\nDigite os elementos da segunda lista:")
    for i in range(10):
        elemento = input(f"Digite o {i+1}º elemento: ")
        lista2.append(elemento)
    
    # Inicializando a terceira lista vazia
    lista3 = []
    
    # Intercalando os elementos das duas listas
    for i in range(10):
        lista3.append(lista1[i])
        lista3.append(lista2[i])
    
    # Mostrando a terceira lista
    print("\nTerceira lista com elementos intercalados:")
    print(lista3)
    ```
<hr>

11. **Altere o programa anterior, intercalando 3 listas de 10 elementos cada.**

    ```python
    # Intercalador de Listas Versão 2.0
    # Declaração de Variáveis
    
    # Inicializando três listas vazias para armazenar os elementos das listas
    lista1 = []
    lista2 = []
    lista3 = []
    
    # Lendo os elementos da primeira lista
    print("Digite os elementos da primeira lista:")
    for i in range(10):
        elemento = input(f"Digite o {i+1}º elemento: ")
        lista1.append(elemento)
    
    # Lendo os elementos da segunda lista
    print("\nDigite os elementos da segunda lista:")
    for i in range(10):
        elemento = input(f"Digite o {i+1}º elemento: ")
        lista2.append(elemento)
    
    # Lendo os elementos da terceira lista
    print("\nDigite os elementos da terceira lista:")
    for i in range(10):
        elemento = input(f"Digite o {i+1}º elemento: ")
        lista3.append(elemento)
    
    # Inicializando a quarta lista vazia
    lista_final = []
    
    # Intercalando os elementos das três listas
    for i in range(10):
        lista_final.append(lista1[i])
        lista_final.append(lista2[i])
        lista_final.append(lista3[i])
    
    # Mostrando a quarta lista
    print("\nQuarta lista (elementos intercalados das três primeiras listas):")
    print(lista_final)
    ```
<hr>

## Fundamentos de Algoritmo

Acesse o repositório principal: https://github.com/devitruvius/ADS-fundamentos-de-algoritmos
