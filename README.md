# Projeto: Dados dos Atletas

## Dica: Lembra sempre de iniciar no terminal, não abre direto no vs

## Descrição

Este projeto foi desenvolvido como parte da certificação DEVStart – Geração Caldeira, com o objetivo de criar uma aplicação em JavaScript capaz de registrar informações de atletas, calcular seus parâmetros físicos e de desempenho, e exibir os resultados formatados no console.

O programa utiliza orientação a objetos, concentrando os dados e comportamentos dentro de uma classe chamada Atleta.

## Funcionalidades

A classe Atleta recebe os seguintes atributos:

nome

idade

peso

altura

notas (array de números)

E possui os seguintes métodos:

calculaCategoria() → determina a categoria do atleta conforme a idade

calculaIMC() → calcula o Índice de Massa Corporal

calculaMediaValida() → calcula a média das notas descartando a maior e a menor

Métodos “getters” como obtemNomeAtleta(), obtemIMC(), etc.

exibirInformacoes() → exibe todas as informações do atleta formatadas no console

## Regras de Cálculo

| Faixa etária  | Categoria     |
| ------------- | ------------- |
| 9 a 11 anos   | Infantil      |
| 12 a 13 anos  | Juvenil       |
| 14 a 15 anos  | Intermediário |
| 16 a 30 anos  | Adulto        |
| Outras idades | Sem categoria |

## IMC

Fórmula:

IMC = Peso
    ---------
 (altura x altura)

 Média Válida

Desconsidera-se a maior e a menor nota, somando as demais e dividindo pelo número restante de notas.

## Exemplo de Uso

// Declara o atleta
const atleta = new Atleta("Cesar Abascal", 30, 80, 1.70, [10, 9.34, 8.42, 10, 7.88]);

// Exibe as informações no console
atleta.exibirInformacoes();

Saída esperada:
Nome: Cesar Abascal
Idade: 30
Peso: 80
Altura: 1.7
Notas: 10,9.34,8.42,10,7.88
Categoria: Adulto
IMC: 27.68166089965398
Média válida: 9.253333333333332

## Estrutura do Projeto

dados-atletas/
│
├── dados-atletas.js   # Arquivo principal com a classe e a execução
└── README.md           # Este arquivo

Como Executar

Instale o Node.js

Clone o repositório:

git clone [git@github.com:aKethelen/dados-atletas.git](https://github.com/aKethelen/dados-atletas.git)

Entre na pasta do projeto:

cd dados-atletas

Execute o código:

node dados-atletas.js

## Tecnologias Utilizadas

JavaScript (ES6+)

Node.js

VS Code para desenvolvimento

## Autor

Kethelen de Azevedo
Desenvolvido para a certificação DEVStart – Geração Caldeira
Projeto orientado a objetos com foco em boas práticas e clareza de código.
