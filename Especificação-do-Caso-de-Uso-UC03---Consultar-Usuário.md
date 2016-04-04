# **UC03 - Consultar Usuário**

##  ***#PartiuFormar***

### **Versão 1.4**

### Histórico da Revisão
Data|Versão|Descrição|Autor
-----|------|---------|-------
28/03/2016|1.0|Criação do documento|Hugo Martins

#### 1. Caso de Uso: UC03 - Consultar Usuário

## Descrição

Este caso de uso permite a consulta de um usuário.

## Ator

Usuário

##Pré-Condições

Usuário autenticado.

## Fluxo Básico 
1. O Usuário escolhe a opção de consultar usuários. 
2. O sistema solicita ao Usuário os dados do aluno para consulta.
3. O Usuário preenche os campos para consulta.
4. O sistema valida e apresenta os resultados da consulta. [FE01]()
5. O Usuário seleciona o aluno que deseja.
6. O sistema apresenta os dados do aluno.
7. O caso de uso é encerrado..
	
## Fluxos Alternativos
Não há.

## Pós Condições
* Usuário consultado.

## Fluxo de Exceção
FE01 - Usuário não encontrado
1. O sistema apresenta uma mensagem para o usuário informando que o usuário n]ao foi encontrado.
2. O caso de uso retorna ao passo 2 do Fluxo Básico.