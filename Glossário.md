# **Glossário**

##  ***#PartiuFormar***
   
### **Versão 1.0**

### Histórico da Revisão
Data|Versão|Descrição|Autor
-----|------|---------|-------
31/03/2016|0.1|Introdução, Finalidade, Escopo, Definições 2.1, 2.2, 2.3|Eduardo Brasil
31/03/2016|0.2|Definições 2.4, Referencias Bibliográficas |Eduardo Brasil

#### 1. Introdução

As especificações apresentadas em toda documentação do sistema **#PartiuFormar** possuem termos pouco conhecidos por pessoas não familiarizados com informatica, deste modo este documento tem como objetivo facilitar o entendimento de todos sobre os termos e palavras chaves que serão utilizados na documentação do **#PartiuFormar**.

##### 1.1 Finalidade
Apresentar ao leitor de todos os termos referentes aos artefatos gerados pelo **#PartiuFormar** e a definição de termos técnicos do mesmo.   

##### 1.2 Escopo

Encontra-se neste documento todas as definições e explicações necessárias para total entendimento dos termos utilizados na documentação do sistema **#PartiuFormar**

##### 1.3 Visão Geral

#### 2. Definições

##### 2.1 Ator

• Usuário ou sistema atuante em funcionalidades do projeto, interage com os Casos de Uso
do sistema e podem validá-los de acordo com a necessidade.

• Pode ser encontrado em todos os documentos referentes ao **#PartiuFormar**, observando a representação do mesmo no documento de Modelagem de Casos de Uso, presente também no Documento de
Visão.

##### 2.2 Caso de Uso

• Representa uma funcionalidade do sistema, é comum sua representação em forma de Modelagem de Casos
de Uso, apresentando as funcionalidades (Casos de Uso) e os Atores que interagem com cada caso de uso.

• Pode ser encontrado na Modelagem de Casos de Uso e na Especificação de Casos de Uso.

##### 2.3 CRUD

• Create, Read, Update e Delete, também conhecido como C.R.U.D, serão operações que serão utilizadas ao longo do projeto.

##### 2.4 IRA
 
• O Índice de Rendimento Acadêmico (IRA) avalia o desempenho dos estudantes ao longo do curso. Para calcular o IRA, que varia de 0 a 5, são consideradas as menções obtidas e o número de créditos das disciplinas cursadas pelo aluno, bem como o trancamento de matérias optativas e obrigatórias.(UnB,2016)

O calculo do IRA é realizado da seguinte forma:

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




## Referencias Bibliográficas

Universidade de Brasilia acesso em: 31/03/2016 <http://www.unb.br/administracao/diretorias/dds/index2.php>

Universidade de Brasilia acesso em: 31/03/2016 <http://www.unb.br/administracao/decanatos/deg/downloads/index/guia_calouro_2_2011.pdf>