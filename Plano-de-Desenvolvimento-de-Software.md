# **Plano de Desenvolvimento de Software**

##  ***#PartiuFormar***

### **Versão 1.1**

### Histórico da Revisão
Data|Versão|Descrição|Autor
-----|------|---------|-------
03/04/2016|1.0|Criação do documento|Hugo Martins
03/04/2016|1.1|Preenchimento dos itens de introdução, finalidade, escopo, referências, visão geral, visão geral do projeto, organização do projeto, e alguns itens do processo de gerenciamento|Hugo Martins

#### 1.                  Introdução

Este documento apresenta o plano de desenvolvimento de _software_ utilizado para o desenvolvimento do sistema #PartiuFormar.

##### 1.1               Finalidade

Este documento tem por finalidade definir aspectos em comuns em planos de desenvolvimento de _software_ para organizar o desenvolvimento do software a fim de que todos os envolvidos no projeto tenham conhecimento de como se trabalhar.

##### 1.2               Escopo

Este plano está dividido em três aspectos:

* Processo de desenvolvimento de software adotado: Processo Unificado Ágil (AUP);
* Definições gerais;
* Visão do Sistema.

##### 1.3               Definições, Acrônimos e Abreviações



##### 1.4               Referências

>>[Documento de Visão](https://github.com/vitornere/vouformar/wiki/Documento-de-Vis%C3%A3o)

##### 1.5               Visão Geral

Este documento está dividido em três itens importantes para um desenvolvimento de _software_:
* Visão geral do projeto;
* Organização do projeto;
* Processo de gerenciamento

#### 2.                  Visão Geral do Projeto

##### 2.1               Finalidade, Escopo e Objetivos do Projeto

O projeto tem como objetivo desenvolver um sistema que permite que o aluno possa, desde o início de sua graduação, realizar um plano de curso onde, a partir das matérias disponíveis, ser possível organizar e criar metas para cada semestre. Poderá acompanhar seu rendimento acadêmico e estimar qual será seu rendimento após um semestre. Além de poder compartilhar seu planejamento no perfil e poder pesquisar por planejamentos compartilhados mais comuns

##### 2.2               Suposições e Restrições

O desenvolvimento do projeto possui apenas restrição de prazo que tem uma data de entrega determinada: 24 de junho de 2016.

##### 2.3               Produtos Liberados do Projeto

O projeto possui como entregáveis os seguintes artefatos:
Documento de Visão;
Documento de Arquitetura de _Software_;
Regras de Negócio;
Especificação Suplementar;
Glossário;
Modelo de Domínio;
Diagrama de Classes;
Diagrama de Atores;
Diagrama de Casos de Uso;
Especificação de Casos de Uso;
Diagrama de Sequência;
Diagrama de Classes;
Incremento de _Software_.

##### 2.4               Evolução do Plano de Desenvolvimento de Software

Este plano será refinado e incrementado a cada iteração de desenvolvimento do _software_.

#### 3.                  Organização do Projeto
##### 3.1               Estrutura Organizacional

A equipe de trabalho do projeto foi planejada de maneira com que todos da equipe trabalhem de maneira igualitária. Assim foi definido que para planejar e gerenciar o acompanhamento da iteração, a mesma terá uma dupla de gerentes que será mudada a cada iteração de acordo com a esquemática definida pela equipe de acordo com a tabela abaixo:

Iterações Ímpares: |Iterações pares:
------------ | ------------------
Hugo Martins e Vitor Nere|Eduardo Brasil e Jonnatas Lennon

##### 3.2               Papéis e Responsabilidades
Pessoa|Papel
------------ | -------------|
Eduardo Brasil|Agile Modeler, Gerente de Configuração, Escritor técnico, Desenvolvedor e _Tester_
Hugo Martins|Agile Modeler, Gerente de Configuração, Escritor técnico, Desenvolvedor e _Tester_
Jonnatas Lennon|Agile Modeler, Gerente de Configuração, Escritor técnico, Desenvolvedor e _Tester_
Vitor Nere|Agile Modeler, Gerente de Configuração, Escritor técnico, Desenvolvedor e _Tester_

#### 4.                  Processo de Gerenciamento

Nesta seção estão descritos alguns tópicos acerca do processo de gerenciamento do projeto, tais como estimativas de prazo, planos de fase, planejamento de _Releases_ e recursos do projeto.
	
##### 4.1               Estimativas do Projeto
Prazo|96 dias
-------|---------------|----
Data inicial:|21/03
Data final:| 24/06

#### 4.2               Plano do Projeto

O projeto está dividido em seis iterações. Cada iteração passa pelas quatro fases do processo de desenvolvimento de _software_ utilizado: Concepção, Elaboração, Construção e Transição.

##### 4.2.1          Plano de Fase
Iteração|Casos de Uso|Objetivos|Data de início|Data de Fim
-------|---------------|------------------------------------------------------------------------------------------|---------|----------
01|UC01 UC02 UC03 UC04|Artefatos da fase de Concepção e iniciar alguns artefatos da fase de Elaboração e immplementar incremento de software|21/03|04/04
02|||04/04|17/04
03|||18/04|01/05
04|||02/05|15/05
05|||16/05|29/05
06|||30/05|12/06

##### 4.2.2     Releases     

O projeto foi planejado em duas _Releases_, sendo a primeira trazendo a funcionalidade principal do planejamento do fluxo e a segunda com as funcionalidades de planejar grade horária e estimar IRA.

Release|Características|Data
-------|---------------|----
01|Registro de Usuários, Registro de Disciplinas, Registro de Turmas e Planejar Fluxo|16/05
02|Planejar Grade e Estimar IRA|13|06

##### 4.2.3          Programação do Projeto

Marcos com pontos de controle do projeto por parta da interessada Milene Serrano:

Descrição|Data
---------|----------
Entrega 01|04/04
Entrega 02|06/05
Entrega 03|30/05
Entrega Final|24/06
	
##### 4.2.4          Recursos do Projeto

O Recurso Humano do projeto possui uma equipe com quatro membros:

* Eduardo Brasil;
* Hugo Martins;
* Jonnatas Lennon;
* Vitor Nere.

##### 4.3               Controle e Monitoramento do Projeto

Nesta serão serão listados e descritos os itens a serem monitorados e controlados pelo projeto:

**Gerenciamento de Requisitos:**

Os requisitos do projeto serão gerenciados através de _Issues_ no repositório do GitHub.

**Gerenciamento de Riscos:**

Classificação de probabilidade (Alta, Média, Baixa)|Classificação de impacto (Alto, Médio, Baixo)|Impacto e Descrição do Risco|Estratégia de Diminuição e/ou Plano de Contingência|Ação a ser tomada
----------------|-----------------|----------------|-----------------|------------------
Baixa|Alto|Membro da equipe sair do projeto|Integração e motivação da equipe| Redesignar atividades do membro desistente aos outros integrantes da equipe
Média|Alto|Atraso no desenvolvimento das atividades|Deixar um _buffer_ de tempo em cada iteração para caso ocorra atrasos|Realocar atividades considerando o _buffer_ de tempo no cronograma
Baixa|Médio|Mudança no Escopo|Deixar um _buffer_ de tempo em cada iteração para caso ocorra mudanças|
Baixa|Alto|Suspensão do calendário acadêmico||Avaliar as mudanças ocorridas para realocar as atividades dessas mudanças nas próximas iterações.

**Gerenciamento de Configuração:**

Informações do Gerenciamento de Configuração pode ser visualizada no >>[Plano de Desenvolvimento de Software](https://github.com/vitornere/partiuformar/wiki/Plano-de-Desenvolvimento-de-Software)

**Ambiente:**
Versão do Ruby: 2.3.0
Versão do Rails: 4.2.6
Teste:
Cobertura de Código:
Versão do Banco de Dados: