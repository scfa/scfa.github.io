# **UC02 - Editar Usuário**

##  ***#PartiuFormar***

### **Versão 1.4**

### Histórico da Revisão
Data|Versão|Descrição|Autor
-----|------|---------|-------
28/03/2016|1.0|Criação do documento|Hugo Martins

#### 1. Caso de Uso: UC02 - Editar Usuário

## Descrição

Este caso de uso permite a edição de um usuário.

## Ator

Usuário

##Pré-Condições

Usuário autenticado no sistema.

## Fluxo Básico 

1. O usuário escolhe a opção de consultar usuário.

2. O Usuário escolhe a opção para alterar uma usuário.

3. O sistema exibe os dados atuais do usuário. [[RN03](https://github.com/vitornere/partiuformar/wiki/Regras-de-Neg%C3%B3cio#usu%C3%A1rios)]
 
4. O Usuário altera o(s) campo(s) desejado(s) e solicita a confirmação da alteração. 

5. O sistema realiza a validação dos dados preenchidos.[[RN01](https://github.com/vitornere/partiuformar/wiki/Regras-de-Neg%C3%B3cio#usu%C3%A1rios), [RN02](https://github.com/vitornere/partiuformar/wiki/Regras-de-Neg%C3%B3cio#usu%C3%A1rios)]
6. sistema realiza a alteração do usuário.
7. O caso de uso é encerrado.

	
## Fluxos Alternativos
Não há.

## Pós Condições
* Usuário criado.

## Fluxo de Exceção
   FE01 - No passo 05 do fluxo básico, o sistema faz a validação dos campos. Caso os campos não estejam de acordo com a [RN01](https://github.com/vitornere/partiuformar/wiki/Regras-de-Neg%C3%B3cio#usu%C3%A1rios) e [RN02](https://github.com/vitornere/partiuformar/wiki/Regras-de-Neg%C3%B3cio#usu%C3%A1rios), o sistema exibe uma mensagem informando o erro ocorrido e volta ao passo 3 do fluxo principal.
