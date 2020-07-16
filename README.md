# Interfaces em Java - Aulão #008
###### DevSuperior - sua carreira dev com fundamento de ensino superior

**Comunidade no Discord**:
https://discord.gg/SbjpsFv

Não perca as novidades:
- https://instagram.com/devsuperior.ig
- https://facebook.com/devsuperior.fb
- https://youtube.com/devsuperior
- https://twitter.com/devsuperior

Assista o vídeo desta aula:

[![Image](https://img.youtube.com/vi/-_ObFKxG30Q/mqdefault.jpg "Vídeo no Youtube")](https://youtu.be/-_ObFKxG30Q)

## Sumário
- [O que você vai aprender](#O-que-você-vai-aprender)
- [Pré-requisitos](#pré-requisitos)
- [Enunciado do exercício](#Enunciado-do-exercício)
- [Exemplo](#Exemplo)
- [Diagramas](#Diagramas)

## O que você vai aprender
- Composição de entidades
- Composição de serviços
- Interfaces
- Inversão de controle / injeção de dependência

## Pré-requisitos

- Lógica de programação
- OOP básica
  - Classes, atributos, métodos, objetos
  - Construtores, encapsulamento
  - List
  - Herança e polimorfismo

## Enunciado do exercício

Uma empresa deseja automatizar o processamento de seus contratos. O processamento de um contrato consiste em gerar as parcelas a serem pagas para aquele contrato, com base no número de meses desejado.

A empresa utiliza um serviço de pagamento online para realizar o pagamento das parcelas. Os serviços de pagamento online tipicamente cobram um juro mensal, bem como uma taxa por pagamento. Por enquanto, o serviço contratado pela empresa é o do Paypal, que aplica juros simples de 1% a cada parcela, mais uma taxa de pagamento de 2%.

Fazer um programa para ler os dados de um contrato (número do contrato, data do contrato, e valor total do contrato). Em seguida, o programa deve ler o número de meses para parcelamento do contrato, e daí gerar os registros de parcelas a serem pagas (data e valor), sendo a primeira parcela a ser paga um mês após a data do contrato, a segunda parcela dois meses após o contrato e assim por diante. Mostrar os dados das parcelas na tela.

## Exemplo

![myImage](https://github.com/devsuperior/aulao008/raw/master/example.png)

### Cálculos

```
Parcela #1: 
200 + 1% * 1 = 202 
202 + 2% = 206.04
```

```
Parcela #2: 
200 + 1% * 2 = 204 
204 + 2% = 208.08
```

```
Parcela #3: 
200 + 1% * 3 = 206 
206 + 2% = 210.12
```

## Diagramas

### Entidades

![myImage](https://github.com/devsuperior/aulao008/raw/master/entities.png)

### Serviços

![myImage](https://github.com/devsuperior/aulao008/raw/master/services.png)
