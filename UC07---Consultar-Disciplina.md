# **UC07 - Consultar Disciplina**

##  ***#PartiuFormar***

### **Versão 1.0**

### Histórico da Revisão
Data|Versão|Descrição|Autor
-----|------|---------|-------
26/04/2016|1.0|Criação do documento|Eduardo Brasil

#### 1. Caso de Uso: UC07 - Consultar Disciplina

## Descrição

Este caso de uso permite a consulta de uma Disciplina.

## Ator

Usuário

##Pré-Condições

Usuário autenticado.

## Fluxo Básico 
1. O Usuário escolhe a opção de consultar Disciplinas. 
2. O sistema solicita ao Usuário os dados da disciplina para consulta.
3. O Usuário preenche os campos para consulta.
4. O sistema valida e apresenta os resultados da consulta. [[FE01](https://github.com/vitornere/partiuformar/wiki/UC07---Consultar-Disciplina/_edit#fluxo-de-exce%C3%A7%C3%A3o)]
5. O Usuário seleciona a disciplina que deseja consultar.
6. O sistema apresenta os dados da disciplina.
7. O caso de uso é encerrado..
	
## Fluxos Alternativos
Não há.

## Pós Condições
* Disciplina consultada.

## Fluxo de Exceção
FE01 - Disciplina não encontrada

1. O sistema apresenta uma mensagem para o usuário informando que a disciplina não foi encontrada.
2. O caso de uso retorna ao passo 2 do Fluxo Básico.
