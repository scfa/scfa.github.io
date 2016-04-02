# **Especificação de Caso de Uso: Manter Usuário**

##  ***#PartiuFormar***

### **Versão 1.0**

### Histórico da Revisão
Data|Versão|Descrição|Autor
-----|------|---------|-------
22/03/2016|1.0|Especificação do caso de Uso|Jônnatas

# UC 001 – MANTER USUÁRIOS
## DESCRIÇÃO

Este caso de uso irá permitir o Usuário crie, altere, consulte e exclua alunos no sistema.

## ATORES

Usuário

##PRECONDIÇÕES

O Usuário deve estar cadastrado no sistema como Usuário.

## FLUXO BÁSICO (FB) 

1. O sistema apresenta as opções
* Consultar usuários. [FB]
* Cadastrar usuários. [FA01]
2. O Usuário escolhe a opção de consultar usuários. 
3. O sistema solicita ao Usuário os dados do aluno para consulta. [RN02]
4. O Usuário preenche os campos para busca.
5. O sistema valida e apresenta os resultados da consulta. [FE01]
6. O Usuário seleciona o aluno que deseja.
7. O sistema apresenta os dados do aluno.
8. O sistema apresenta as opções para:
* Concluir a consulta.
* Deletar dados. [FA02]
* Alterar dados.[FA03]
9. O caso de uso é encerrado.	

## FLUXOS ALTERNATIVOS
5.1 FA01 – Cadastrar aluno

1. O sistema solicita ao Usuário o preenchimento dos campos para o cadastro. [RN01]
2. O Usuário preenche os campos e solicita a confirmação do cadastro.
3. O sistema realiza a validação dos dados preenchidos. [RN01] [FE02] [FE03]
4. sistema realiza o cadastro do aluno.
5. O caso de uso é encerrado.

5.2 FA02 – Excluir dados

1. O Usuário escolhe a opção para excluir uma aluno.
2. O sistema apresenta uma mensagem de confirmação de exclusão. [ME01]
3. O Usuário confirma a exclusão
4. O caso de uso retorna ao passo 8 do FB.

5.3 FA03 – Alterar dador

1. O Usuário escolhe a opção para alterar uma aluno.
2. O sistema exibe os dados atuais dos alunos.
3. O Usuário altera o(s) campo(s) desejado(s) e solicita a confirmação da alteração. [RN01] 
4. O sistema realiza a validação dos dados preenchidos. [RN01] [FE02] [FE03]
5. O caso de uso retorna ao passo 8 do FB.

## FLUXOS DE EXCEÇÃO

6.1 FE01 - O sistema não encontra uma aluno
1. O sistema apresenta uma mensagem para o usuário.  [ME02]
2. O caso de uso retorna ao passo 2 do FB.

6.2 FE02 - Campos para cadastro preenchidos incorretamente

1. Este fluxo pode ser chamado nos passos:
* Passo 3 do FA01
* Passo 4 do FA03
2. O sistema encontra algum erro na validação dos dados.
3. O sistema apresenta uma mensagem de erro. [ME03]
4. O caso de uso retorna ao fluxo de origem.

6.3 FE03 - Campos obrigatório em branco no cadastro.

1. Este fluxo pode ser chamado nos passos:
* Passo 3 do FA01.
* Passo 4 do FA03
2. O sistema encontra algum erro na validação dos dados.
3. O sistema apresenta uma mensagem de erro. [ME04]
4. O caso de uso retorna ao fluxo de origem.

## PÓS-CONDIÇÕES
* Nenhuma ou muitas aluno, tiveram seus registros alterados/incluídos no banco de dados.

## MENSAGEM.
* ME01 - “Deseja confirmar a exclusão?”
* ME02 - “Nenhuma aluno foi encontrado”
* ME03 - “Campos preenchidos incorretamente”
* ME04 - “Todos os campos obrigatórios devem ser preenchidos”

## REGRAS DE NEGÓCIO.
 