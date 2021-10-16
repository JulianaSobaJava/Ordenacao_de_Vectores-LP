# Ordenacao_de_Vectores-LP

Faça um algoritmo para ler 10 números e armazenar em um vetor. Após isto, o
algoritmo deve ordenar os números no vetor em ordem crescente. No final, deve
ser lido mais um número qualquer e inserir esse novo número na posição correta,
ou seja, mantendo a ordem crescente do vetor. Escrever o vetor ordenado.
Upgraded by:Professor José Gonçalves;


Algoritmo "Ordenar"
var

   vet: vetor[1..11] de inteiro
   i,j,aux,plus:inteiro
   
   //---------------------Inicio do Procedimento --------------------------
   
procedimento ordenar(length:inteiro)
var
   i,j,aux:inteiro
inicio

   para i de 1 ate length faca
      para j de 1 ate length-1 faca
         se vet[i]<vet[j] entao
            aux<-vet[i]
            vet[i]<-vet[j]
            vet[j]<-aux
         fimse
      fimpara
   fimpara
   escreval("")
   para i de 1 ate length faca
      escreval(vet[i])
   fimpara
fimprocedimento


//---------------------Fim do Procedimento --------------------------

Inicio

   para i de 1 ate 10 faca
      leia(vet[i])
   fimpara
   ordenar(10)
   escreva("Digite um valor:")
   leia(plus)
   vet[11]<-plus
   ordenar(11)
Fimalgoritmo
