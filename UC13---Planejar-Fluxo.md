# **UC13 - Planejar Fluxo**

##  ***#PartiuFormar***

### **Versão 1.0**

### Histórico da Revisão
Data|Versão|Descrição|Autor
-----|------|---------|-------
24/06/2016| 1.0 |Criação do Documento | Hugo Martins

#### 1. Caso de Uso: UC13 - Planejar Fluxo

## Descrição

Este caso de uso permite a realização do planejamento de um novo Fluxo.

## Ator

Usuário

##Pré-Condições

Usuário deverá está logado no sistema.

## Fluxo Básico 
1. O Usuário do Sistema escolhe a opção de Planejar Fluxo.
2. O sistema exibe ao Usuário uma lista de disciplinas e um checkBox com os semestres para cada disciplina[[RN07](https://github.com/vitornere/partiuformar/wiki/Regras-de-Neg%C3%B3cio#fluxo)].
3. O Usuário seleciona a disciplina que gostaria de alocar.
4. O usuário seleciona no checkBox o número do semestre a qual gostaria de alocar a disciplina. 
5. O usuário clica no botão confirmando o registro do novo Fluxo.
9. O caso de uso é encerrado.
	
## Fluxos Alternativos

* 4a Não existe nenhuma disciplina cadastrada no sistema
 1. Retorna uma mensagem ao usuário na tela informando que não existe nenhuma disciplina a ser selecionada.

## Pós Condições
* Plano de Fluxo criado.

## Fluxo de Excessão
* Não há.