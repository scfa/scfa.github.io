# **UC06 - Editar Disciplina**

##  ***#PartiuFormar***

### **Versão 1.0**

### Histórico da Revisão
Data|Versão|Descrição|Autor
-----|------|---------|-------
26/04/2016|1.0|Criação do documento| Eduardo Brasil


#### 1. Caso de Uso: UC06 - Editar Disciplina

## Descrição

Este caso de uso permite a edição de uma disciplina.

## Ator

Administrador do sistema 

##Pré-Condições

A disciplina deve esta cadastrada no sistema.

## Fluxo Básico 

1. O usuário escolhe a opção de consultar disciplina.

2. O Usuário escolhe a opção para alterar uma disciplina.

3. O sistema exibe os dados atuais da disciplina. [[RN06](https://github.com/vitornere/partiuformar/wiki/Regras-de-Neg%C3%B3cio#disciplinas)]
 
4. O Usuário altera o(s) campo(s) desejado(s) e solicita a confirmação da alteração. 

5. O sistema realiza a validação dos dados preenchidos.[[RN05](https://github.com/vitornere/partiuformar/wiki/Regras-de-Neg%C3%B3cio#disciplinas)]
6. sistema realiza a alteração da Disciplina.
7. O caso de uso é encerrado.

	
## Fluxos Alternativos
1. Código da disciplina não está cadastrada no Sistema.

1.1 O sistema retorna uma mensagem informando que a Disciplina não existe e retorna a página de busca.

## Pós Condições
* Disciplina Alterada.

## Fluxo de Exceção
   FE01 - No passo 05 do fluxo básico, o sistema faz a validação dos campos. Caso os campos não estejam de acordo com a [[RN05](https://github.com/vitornere/partiuformar/wiki/Regras-de-Neg%C3%B3cio#disciplinas)] 
