# **UC09 - Planejar Grade Horária**

##  ***#PartiuFormar***

### **Versão 1.0**

### Histórico da Revisão
Data|Versão|Descrição|Autor
-----|------|---------|-------
23/05/2016| 1.0 |Criação do Documento | Hugo Martins

#### 1. Caso de Uso: UC09 - Planejar Grade Horária

## Descrição

Este caso de uso permite a realização do planejamento de uma nova grade horária.

## Ator

Usuário

##Pré-Condições

Usuário deverá está logado no sistema

## Fluxo Básico 
1. O Usuário do Sistema escolhe a opção de Planejar Grade Horária.
2. O sistema exibe ao Usuário uma grade de horários vazios para preenchimento de disciplinas.
3. O Usuário seleciona o horário que quer alocar uma disciplina e clica no botão dentro da grade que indica tal horário.
4. O sistema encaminha o usuário para a lista de disciplinas cadastradas. [[RN09](https://github.com/vitornere/partiuformar/wiki/Regras-de-Neg%C3%B3cio#grade)]
5. O usuário seleciona a disciplina desejada.
6. O sistema volta para a tela da grade horária com a disciplina escolhida já incluída na grade.
7. Os passos 3, 4, 5, 6 e 7 são repetidos quantas vezes necessárias pelo usuário.
8. O usuário clica no botão de registro da grade horária.
9. O sistema valida as informações.
6. O caso de uso é encerrado.
	
## Fluxos Alternativos

* 4a Não existe nenhuma disciplina cadastrada no sistema
 1. Retorna uma mensagem ao usuário na tela informando que não existe nenhuma disciplina a ser selecionada.

## Pós Condições
* Plano de grade horária criado.

## Fluxo de Excessão
* Não há.