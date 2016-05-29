# **Regras de Negócio**

##  ***#PartiuFormar***
   
### **Versão 1.3**

### Histórico da Revisão
Data|Versão|Descrição|Autor
-----|------|---------|-------
21/03/2016|1.0|Criação do documento|Hugo Martins / Jônnatas Lennon / Vitor Nere
27/03/2016|1.1|Adicionado novas regras|Vitor Nere
03/04/2016|1.2|Revisando o documento|Hugo Martins
29/05/2016|1.3|Refinando o documento|Hugo Martins

#### 1.                  Introdução

Esse documento descreve todas as regras de negócio referentes ao sistema #PartiuFormar. 

##### 1.1               Finalidade
Esse documento tem por objetivo descrever as regras de negócio estabelecidas no sistema acadêmico da Universidade de Brasília (UnB), no qual o sistema será acoplado.   

##### 1.2               Escopo

Para este plano foram considerados os aspectos da Visão do sistema.

##### 1.3               Referências

[Matricula Web](https://matriculaweb.unb.br)

##### 1.4               Visão Geral

Este artefato está dividido nas seguintes seções: Introdução, Definições e Descrição das Regras de Negócio.

#### 2.                  Definições

Nesta seção serão listadas as regras de negócios que devem ser atribuídas ao sistema para o seu correto funcionamento. Cada Regra de negócio está identificada por um código denominado RN e o número da mesma. 

##### Usuários

ID| Descrição
-----|----------------------------------------------------------------
RN01|O usuário durante a realização do cadastro no sistema, deverá informar uma matrícula válida pela UnB a qual deverá ser única.
RN02|A senha do usuário deve ser no mínimo de 8 caracteres, possuindo letras e números, podendo conter caracteres especiais. 
RN03| No formulário do cadastro, deverá conter dois campos para a validação da senha, sendo obrigatório o preenchimento.
RN04 - Campos a serem preenchidos no cadastro:

Campo|Formato|Obrigatoriedade
-----|-------|-----
Nome do Aluno|Texto|Sim
Sobrenome|Texto|Não
Matricula|nn/nnnnnnn|Sim
Semestre atual|nn|Não
Semestre de ingresso|nn/nnnn|Sim
Email|x at x dot com|Sim
Curso|Combobox de cursos|Sim
Senha|RN 02|Sim

##### Disciplinas
ID| Descrição
-----|----------------------------------------------------------------
RN05|O código da disciplina deve ser único e só poderá ser cadastrado pelo administrador do sistema.

RN06 - Campos a serem preenchidos no cadastro de uma disciplina.

Campo|Formato|Obrigatoriedade
-----|-------|-----
Denominação|Texto|SIM
Ementa|Texto|Sim
Código|xxxxxxx|Sim
Créditos|xxxxxxx|Sim
Departamento|comboboox de departamento|Sim
Turma|Texto|Sim
Turno|Texto|Sim
Horário|Texto|Sim
Local|Texto|Sim
Professor|Combobox de Professor|Sim
Pré-Requisitos|Texto|Não

##### Fluxo
ID| Descrição
-----|----------------------------------------------------------------
RN07|Um fluxo padrão é gerado a partir da escolha do curso pelo aluno.

##### Grade
ID| Descrição
-----|----------------------------------------------------------------
RN008|Uma grade padrão é gerada a partir do planejamento de fluxo e o semestre cursado pelo aluno.
RN009|Só é permitido a criação de um plano de grade horária se existir ao menos uma disciplina cadastrada no sistema.

##### IRA
ID| Descrição
-----|----------------------------------------------------------------
RN010|O cálculo do IRA (Índice de Rendimento Acadêmico) é baseado na fórmula retirada do guia do calouro e pode ser alterada semestralmente, abaixo encontra-se como é realizado o cálculo: 

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