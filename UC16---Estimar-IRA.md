# **UC16 - Estimar IRA**

##  ***#PartiuFormar***

### **Versão 1.0**

### Histórico da Revisão
Data|Versão|Descrição|Autor
-----|------|---------|-------
24/06/2016| 1.0 |Criação do Documento | Hugo Martins

#### 1. Caso de Uso: UC15 - Excluir Fluxo

## Descrição

Este caso de uso permite que o usuário faça um estimativa de seu IRA (Índice de Rendimento Acadêmico) ao final do semestre.

## Ator

Usuário

##Pré-Condições

Usuário autenticado no sistema. 

## Fluxo Básico 

1. O Usuário seleciona a opção de Estimar IRA.
2. O Usuário seleciona o semestre para a realização da estimativa.
3. O sistema apresenta um formulário com os dados necessários para a realização do cálculo.
4. O Usuário informa a quantidade de créditos da disciplina e a menção.
5. O Usuário seleciona a opção para adicionar uma nova disciplina.
6. Os passo 4 e 5 são realizado pelo Usuário quantas vezes necessário.
7. O Usuário seleciona a opção para fazer o calculo do IRA [[RN010](https://github.com/vitornere/partiuformar/wiki/Regras-de-Neg%C3%B3cio#ira)].
8. O sistema exibe uma mensagem informando o valor do IRA estimado.
9. O caso de uso é encerrado.
	
## Fluxos Alternativos

Não há

## Pós Condições
 Novo IRA estimado.