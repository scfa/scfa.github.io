# **UC05 - Criar Disciplina**

##  ***#PartiuFormar***

### **Versão 1.1**

### Histórico da Revisão
Data|Versão|Descrição|Autor
-----|------|---------|-------
11/04/2016| 1.0 |Criação do Documento | Eduardo Brasil
04/05/2016| 1.1 |Refinando documento | Hugo Martins

#### 1. Caso de Uso: UC05 - Criar Disciplina

## Descrição

Este caso de uso permite a criação de uma nova disciplina.

## Ator

Administrador do sistema

##Pré-Condições

Administrador do Sistema devera esta logado no sistema

## Fluxo Básico 
1. O Administrador do Sistema escolhe a opção de criar Disciplina
2. O sistema exibe ao Administrador do Sistema um formulário de criação. [[RN06](https://github.com/vitornere/partiuformar/wiki/Regras-de-Neg%C3%B3cio#disciplinas)]
3. O Administrador do sistema preenche os campos e solicita a confirmação do cadastro da disciplina.
4. O sistema realiza a validação dos dados preenchidos.[[RN05](O Usuário preenche os campos e solicita a confirmação do cadastro)]
5. sistema realiza o cadastro da Disciplina.
6. O caso de uso é encerrado.
	
## Fluxos Alternativos

* 4a O código da disciplina já esta cadastrado no sistema
 1. Retorna uma mensagem ao Administrador na tela informando que a disciplina já está cadastrada.

## Pós Condições
* Disciplina criada.

## Fluxo de Excessão
  FE01 - No passo 04 do fluxo básico, o sistema faz a validação dos campos. Caso os campos não estejam de acordo com a [RN06](https://github.com/vitornere/partiuformar/wiki/Regras-de-Neg%C3%B3cio#disciplinas) o sistema exibe uma mensagem informando o erro ocorrido e volta ao passo 2 do fluxo principal.
