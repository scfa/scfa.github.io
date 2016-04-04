# **UC01 - Criar Usuário**

##  ***#PartiuFormar***

### **Versão 1.4**

### Histórico da Revisão
Data|Versão|Descrição|Autor
-----|------|---------|-------
28/03/2016|1.0|Criação do documento|Hugo Martins

#### 1. Caso de Uso: UC01 - Criar Usuário

## Descrição

Este caso de uso permite a criação de um novo usuário..

## Ator

Usuário

##Pré-Condições

Não há.

## Fluxo Básico 
1. Usuário escolhe a opção de criar Usuário
2. O sistema exibe ao Usuário o formulário de criação. [[RN03](https://github.com/vitornere/partiuformar/wiki/Regras-de-Neg%C3%B3cio#usu%C3%A1rios)]
3. O Usuário preenche os campos e solicita a confirmação do cadastro.
4. O sistema realiza a validação dos dados preenchidos.[[RN01](https://github.com/vitornere/partiuformar/wiki/Regras-de-Neg%C3%B3cio#usu%C3%A1rios), [RN02](https://github.com/vitornere/partiuformar/wiki/Regras-de-Neg%C3%B3cio#usu%C3%A1rios)]
5. sistema realiza o cadastro do usuário.
6. O caso de uso é encerrado.
	
## Fluxos Alternativos
Não há.

## Pós Condições
* Usuário criado.

## Fluxo de Excessão
  FE01 - No passo 04 do fluxo básico, o sistema faz a validação dos campos. Caso os campos não estejam de acordo com a [RN01](https://github.com/vitornere/partiuformar/wiki/Regras-de-Neg%C3%B3cio#usu%C3%A1rios) e [RN02](https://github.com/vitornere/partiuformar/wiki/Regras-de-Neg%C3%B3cio#usu%C3%A1rios), o sistema exibe uma mensagem informando o erro ocorrido e volta ao passo 2 do fluxo principal.
