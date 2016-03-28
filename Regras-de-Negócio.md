# **Regras de Negócio**

##  ***#PartiuFormar***
   
### **Versão 0.2**

### Histórico da Revisão
Data|Versão|Descrição|Autor
-----|------|---------|-------
21/03/2016|1.0|Criação do documento|Hugo Martins / Jônnatas Lennon / Vitor Nere
27/03/2016|1.0|Adicionado novas regras|Vitor Nere

#### 1.                  Introdução

Esse documento descreve todas as regras de negócio referentes ao sistema #PartiuFormar. 

##### 1.1               Finalidade
Esse documento tem por objetivo descrever as regras de negócio estabelecidas no sistema acadêmico da Universidade de Brasília (UnB), no qual o sistema será acoplado.   

##### 1.2               Escopo

Para este plano foram considerados os aspectos da Visão do sistema.

##### 1.3               Referências

[Matricula Web][UnB]

##### 1.4               Visão Geral

Este artefato está divido nas seções Introdução, Definições e Descrição das Regras de Negócio.

#### 2.                  Definições
Nesta seção serão listadas as regras de negócios que devem ser atribuídas ao sistema para o seu correto funcionamento. Cada Regra de negócio está identificada por um código denominado RN e o número da mesma. 

##### Usuários

ID| Descrição
-----|----------------------------------------------------------------
RN01|O usuário durante a realização do cadastro no sistema, deverá informar uma matrícula válida pela UnB a qual deverá ser única.
RN02|A senha do usuário deve ser no mínimo de 8 caracteres, possuindo letras e números, podendo conter caracteres especiais. 
RN03| No formulário do cadastro, deverá conter dois campos para a validação da senha, sendo obrigatório o preenchimento.

##### Disciplinas
ID| Descrição
-----|----------------------------------------------------------------
RN04|Só poderá ser cadastrada por um administrador do sistema com código único.

##### Fluxo
ID| Descrição
-----|----------------------------------------------------------------
RN05|Um fluxo padrão é gerado a partir da escolha do curso pelo aluno.
RN06|O aluno poderá editar seu fluxo padrão ou criar novos fluxos, podendo decidir qual será seu fluxo padrão.

##### Grade
ID| Descrição
-----|----------------------------------------------------------------
RN07|Uma grade padrão é gerada a partir do planejamento de fluxo e o semestre cursado pelo aluno.
RN08|É possível alterar a grade e o seu estado a qualquer momento.

##### IRA
ID| Descrição
-----|----------------------------------------------------------------
RN09|O cálculo do IRA (Índice de Rendimento Acadêmico) é baseado na fórmula retirada do guia do calouro e pode ser alterada semestralmente, abaixo encontra-se como é realizado o cálculo: ![](http://i.imgur.com/DUna2dt.jpg)