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
<strong>RN04</strong>| Deve obrigatoriamente conter um campo (Obrigatório) preenchidos para executar a consulta.

RN05 - Campos a serem preenchidos no cadastro

Campo|Formato|Obrigatoriedade
-----|-------|-----
Nome do Aluno|TEXT|SIM
Sobrenome|TEXT|NÃO
Matricula|nn/nnnnnnnnn|SIM
Semestre atual|XXXXX|NÃO
Ano de ingrsso|nnnn|SIM
Email|x at x dot com|SIM
Curso|Combobox de cursos|SIM
Senha|RN 02|SIM





##### Disciplinas
ID| Descrição
-----|----------------------------------------------------------------
RN06|Só poderá ser cadastrada por um administrador do sistema com código único.

RN07 - Campos a serem preenchidos no cadastro de uma disciplina.

Campo|Formato|Obrigatoriedade
-----|-------|-----
Denominação|TEXT|SIM
Ementa|TEXT|SIM
Código|xxxxxxx|SIM
Créditos|xxxxxxx|SIM
Departamento|comboboox de departamento|SIM
Turma|TEXT|SIM
Total de Vagas|xxx|SIM
Turno|TEXT|SIM
Horário/Local|TEXT|SIM
Professor|Combobox de Professor|SIM
Pré-Requisitos|TEXT|NÃO
Obs|TEXT|NÃO


##### Fluxo
ID| Descrição
-----|----------------------------------------------------------------
RN08|Um fluxo padrão é gerado a partir da escolha do curso pelo aluno.
RN09|O aluno poderá editar seu fluxo padrão ou criar novos fluxos, podendo decidir qual será seu fluxo padrão.

##### Grade
ID| Descrição
-----|----------------------------------------------------------------
RN010|Uma grade padrão é gerada a partir do planejamento de fluxo e o semestre cursado pelo aluno.
RN011|É possível alterar a grade e o seu estado a qualquer momento.

##### IRA
ID| Descrição
-----|----------------------------------------------------------------
RN012|O cálculo do IRA (Índice de Rendimento Acadêmico) é baseado na fórmula retirada do guia do calouro e pode ser alterada semestralmente, abaixo encontra-se como é realizado o cálculo: 

 **IRA** = { [ 1- (0,6 x DTb + 0,4 x DTp) **/** DC ] **X** [ (Σ Pi x CRi x Pei) **/** (Σ CRi x Pei) ] }

**DTb** = número de disciplinas obrigatórias trancadas

**DTp** = número de disciplinas optativas trancadas

**DC** = número de disciplinas matriculadas
 (incluindo as trancadas)

**Pi** = peso da menção

 (**SS=5, MS=4, MM=3, MI=2, II=1, SR=0**)

**Pei** = período em que uma dada disciplina foi cursada,
obedecendo a seguinte limitação:

 min | 6, período |

**CRi** = número de créditos de uma dada disciplina
Quanto maior for o IRA, maior será a prioridade de
matrícula." (UnB,2016) 