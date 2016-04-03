# **Visão**

##  ***#PartiuFormar***

### **Versão 1.4**

### Histórico da Revisão
Data|Versão|Descrição|Autor
-----|------|---------|-------
21/03/2016|1.0|Introdução, finalidade|Eduardo Brasil
22/03/2016|1.1|Preenchimento dos Itens 1.2 Escopo, 1.3 Visão Geral, 2.1 Descrição do Problema, 2.2 Setença de Posição do Sistema e 3.1 Resumo dos Envolvidos| Vitor Nere
23/03/2016|1.2|Formatação do documento e preenchimento dos ítens 3.2, 3.3, 5.1, 6 e 6.1.| Hugo Martins
24/03/2016|1.3|Edição nos itens 6.1 ; 2.1 ;  3.1 ; 5.2 ; 5.3| Jônnatas Lennon
31/03/2016|1.4|Edição nos itens 2.2, 3.1| Eduardo Brasil

#### 1. Introdução
Este documento tem como intenção, analisar e definir os recursos necessários para realizar com sucesso o desenvolvimento do software **#PartiuFormar**. Para isso, serão necessários a elaboração de alguns artefatos como descrição de caso de uso, diagrama de sequencia e planejamentos das iterações que serão apresentados ao longo deste documento e  que são necessários para satisfazer de forma completa os usuários na utilização deste software.

##### 1.1 Finalidade
Este documento contém os fatores mais relevantes que levarão à construção da do software **#PartiuFormar**. Esse projeto será desenvolvido pelos estudantes da Universidade de Brasília, campus Gama/DF (FGA). Serão apresentadas aqui todas as principais características, finalidades e motivações para o desenvolvimento dessa aplicação, também irá descrever características gerais do sistema, os envolvidos no seu desenvolvimento assim como o publico alvo.

##### 1.2 Escopo
O **#PartiuFormar** permite que o aluno possa, desde o início de sua graduação, realizar um plano de curso onde, a partir das matérias disponíveis, ser possível organizar e criar metas para cada semestre. Poderá acompanhar seu rendimento acadêmico e estimar qual será seu rendimento após um semestre. Além de poder compartilhar seu planejamento no perfil e poder pesquisar por planejamentos compartilhados mais comuns.
##### 1.3 Visão Geral
Faremos uso deste nosso documento como uma forma de organizar informações necessárias para futuras atividades do projeto em desenvolvimento. Informações a cerca do contexto do projeto, funcionalidades, e características serão organizados e estarão disponíveis neste documento afim de poupar o atraso no processo de desenvolvimento do projeto.
##### 1.4 Acrônimos
**1. IRA** - Índice de Rendimento Acadêmico.

**2. UnB** - Universidade de Brasília.

#### 2. Posicionamento

##### 2.1 Descrição do Problema
Surgido por uma necessidade dos estudantes da UnB de organizar uma grade curricular todo semestre, e evitar: 

O problema de|Desorientação, principalmente no início da graduação, de como se organizar e quais matérias cursar a cada semestre, visando uma graduação fluída.
-------------|-------------------------------------
Afeta|Alunos de graduação.
Cujo impacto é|Possibilidade de atros no fluxo, pelo mal planejamento curricular, além de um aproveitamento ineficiente da grade curricular, ocasionando ao aluno uma confusão sobre quais matérias cursar|
Uma solução seria|Uma plataforma que auxilie o aluno no planejamento curricular e tenha todo material para que o aluno se guiar conforme sua instituição

##### 2.2 Sentença de Posição do Sistema

Para|Alunos de graduação
-----|------------------------------
Que|Necessitam acompanhar e monitorar suas grades horarias, cursos e turmas.
O| **#PartiuFormar** auxilia os Alunos
Que|Desejam maior orientação em relação ao rumo da graduação
O **#PartiuFormar**|É um _software_ que possibilita planejar seu currículo e acompanhar a situação, estimando diferentes tipos de estratégia e rendimento acadêmico
Que|Auxilia em uma graduação mais fluída e madura
Diferente de|Do matrícula web que é uma plataforma mais voltada para exibição de informações atuais, da graduação do aluno
Nosso sistema|Será uma base de planejamentos, garantindo maior maturidade para o sucesso da graduação

#### 3. Descrições dos Envolvidos e Usuários

##### 3.1 Resumo dos Envolvidos

Nome|Descrição|Responsabilidades|Interesse|Decisão
----|---------|-----------------|---------|-------------------------------
**Instituições de Ensino Superior**|Instituição na qual o aluno estar matriculado|Prover oferta de matérias semestralmente |Médio|Baixo
**Desenvolvedores e Gerentes**|Profissionais da área que implementarão e integrarão o projeto descrito|Irão produzir o sistema visionado e projetado nos documentos posteriores|Alto|Alto
**Estudantes de Graduação**|Estudante da universidade de Brasilia, os quais utilizarão do sistema para a gestão da sua grade horaria||Alto|Baixo

##### 3.2 Resumo dos Usuários

Nome|Descrição
----|--------------------------------------------------------------------------------
Alunos|Estudantes de graduação na instituição
Professores|Educadores que ministram as disciplinas de graduação
Administradores do Sistema|Responsáveis por manter as informações no sistema

##### 3.3 Principais Necessidades dos Usuários ou dos Envolvidos

Necessidade|Prioridade|Preocupações|Solução Atual|Solução Proposta
-----------|----------|------------|-------------|-----------------------------------------------
Consultar disciplinas|Alta|Deve ser possível a consulta de disciplinas para que o aluno possa obter informações referentes a elas|Existe o campo para consulta de disciplinas no matrícula web|Armazenar dados das disciplinas para que estes fiquem disponíveis para consulta
Simular graduação|Alta|Deve ser permitido que o aluno faça planejamentos de semestres ou de grades horárias futuras|O aluno faz isso  manualmente através das informações de ofertas disponíveis no sistema do matrícula web|Desenvolver no sistema um mecanismo que possibilite ao aluno a realização desse planejamento
Compartilhar Grade horária|Baixa|O aluno deve, quando desejar, informar a outros alunos as disciplinas que está matriculado para que outras pessoas o localizem dentro da universidade|O aluno compartilha sua grade horária com os amigos com o uso de outras tecnologias disponíveis no mercado|Implementar um meio de compartilhamento no sistema
Estimar IRA|Alta|O aluno deve ser capaz de, com base em suas menções, calcular o seu índice de rendimento acadêmico|O aluno faz isso com o auxílio de uma calculadora. A função do índice de rendimento acadêmico muitas vezes não é clara ao aluno ou ele não a conhece|Criar uma função dentro do sistema que calcule o índice de rendimento acadêmico do aluno após o mesmo informar suas menções

* **Alta:** Alta necessidade no sistema deve ser implementado primeiramente.
* **Média:** Necessário ao sistema, porém pode ser implementado posteriormente. 
* **Baixa:** A falta da  implementação não gera gera percas ao sistema, podendo ser implementado por ultimo.

#### 4. Ambiente do Usuário
O sistema será implementado e testado em um servidor web, onde poderá ser acessado de qualquer navegador com acesso a internet.

#### 5. Visão Geral do Sistema

##### 5.1 Perspectiva do Sistema
O sistema tem como objetivo organizar a vida acadêmica de um aluno de graduação para que o mesmo possa fazer planejamentos em relação ao seu curso do semestre vigente e de semestres posteriores até que o mesmo obtenha sua formação.

##### 5.2 Suposições e Dependências
Para a utilização do sistema é suposto que a casa possua conexão com internet.
O usuário precisar ter um conhecimento minimo sobre o funcionamento da instiruição acadêmica.

##### 5.3 Licenciamento e Instalação
Todas as tecnologias utilizadas durante o desenvolvimento e utilização do sistema são **“open-source license”**, ou sejá código aberto.

#### 6. Requisitos Funcionais do Sistema
Esta seção tem a função de informar de forma resumida todas as características e funcionalidades do sistema **#PartiuFormar**.

##### 6.1 Tabela de Requisitos

Requisito|Descrição|Prioridade|Dependência
---------|---------|----------|---------------------------------------------
RF01 - Registrar Usuários|O sistema deve permitir o registro de usuários (Alunos, Professores e Administradores do sistema)|Alta|
RF02 - Registrar Disciplinas|O sistema deve permitir o registro de disciplinas de graduação|Alta|
RF03 - Registrar Turmas|O sistema deve permitir o registro de turmas de uma disciplina|Alta|RF02
RF04 - Planejar Grade Horária do usuário|O sistema deve permitir que o aluno planeje sua grade horária do semestre|Alta|RF01, RF02, RF03
RF05 - Compartilhar Grade Horária do usuário|O sistema deve permitir que o aluno compartilhe com outros usuários a sua grade horária|Baixa|RF01, RF02, RF03, RF04
RF06 - Planejar Fluxo|O sistema deve permitir que o aluno planeje o as disciplinas que pretende se matricular semestre a semestre|Alta|RF01, RF02, RF03
RF07 - Compartilhar Fluxo|O sistema deve permitir que o aluno compartilhe com outros usuários|Baixa|RF01, RF02, RF03, RF06
RF08 - Estimar IRA|O sistema deve permitir que o aluno faça o cálculo de seu índice de rendimento acadêmico|Media|RF01, RF02

#### 7. Requisitos Não Funcionais do Sistema
Vide especificadões suplementares.


#### 8. Referências Bibliográficas