#Plano de Gerenciamento de Configuração e Projeto
##  ***#PartiuFormar***

### **Versão 1.2**

### Histórico da Revisão
Data|Versão|Descrição|Autor
-----|------|---------|-------
21/03/2016|1.0|Criação do documento|Jônnatas Lennon
03/04/2016|1.1|Politica de _branch_|Eduardo Brasil
03/04/2016|1.2|Revisão do documento|Hugo Martins
 

#### 1.                  Introdução
Este documento irá descrever as atividades do Gerenciamento de Controle de Configuração e Mudança (CCM), a serem executadas durante o projeto.

##### 1.1               Finalidade
Este artefato tem como intuito descrever como será desenvolvido o gerenciamento de configuração do _software_ #PartiuFormar, desenvolvido na disciplina Desenho de Software da UnB, detalhando como acontecerá o controle sobre as versões de trabalho produzida ao longo do tempo, bem como suas alterações.

##### 1.2               Escopo

Este modelo segue como inpiração o AUP](http://www.ambysoft.com/unifiedprocess/aup11/html/configurationManagement.html)

##### 1.3               Visão Geral

Esse documento apresenta a ferramenta utilizada, como repositório e seu processo de utilização.

#### 2.                 Ferramentas

Devido a imensa gama de funcionalidades, foi decidido a utilização da ferramenta de versionamento de código, Git, com o serviço GitHub, devido ao mesmo ser amplamente conhecido.

#### 3.                 Repositório 

Nesta seção são tratados assuntos referentes ao repositório do projeto do _software_ #PartiuFormar, tais como organização do diretório, das_ branchs_ e como elas devem ser nomeadas.

##### 3.1               Diretórios

Será mantido duas pastas principais do projeto, a pasta relatório que conterá os relatórios referentes as _releases_ 1 e 2, e a pasta partiuformar que conterá o código desenvolvido.  
    
##### 3.2               Utilização de _branches_ 
      
No projeto serão mantidas duas __branches__: a _master_, a qual armazenará o código estável e revisado, além da _branch_ devel, que armazenará o código a ser desenvolvido, porém sem a devida validação do mesmo. O código só será disponibilizado na _master_ após a aprovação do mesmo pelo responsável pela gerência do código. Além disso, serão criadas _branchs_ chamadas de _Issues_ e cada uma dessas branches será para o desenvolvimento de uma funcionalidade do sistema e a mesmas serão apagadas após seus dados serem passados para a _master_.

#### 3.2.1              Politica de branch

![Extraída e adaptada de A successful git branching model.](http://lappis.unb.br/redmine/attachments/download/2447/branchflow.png)

_Master_
A _branch_ principal que receberá o _merge_ para cada uma das _releases_.

_Devel_
A branch estável que sempre tenta refletir o estado atual do desenvolvimento. Receberá o merge das _branches_ de cada funcionalidade.

_IssueNN_
As _branches_ que são usadas para desenvolver as funcionalidades do sistema, onde "NN" trata-se do número da _Issue_.

O projeto utilizará o sistemas de _issues_ da plataforma GitHub, além do _Kanban_ também disponível no mesmo. Deste modo serão criadas _issues_ para orientar o grupo no desenvolvimento do projeto, a _issue_ deve ter o nome claro referente a sua funcionalidade correspondente, a qual após a conclusão deve ser revisada e acoplada se necessário a _branch_ devel.

##### 3.2.              Nomenclatura.

* Os _commits_ serão escritos em português, devendo ser claros em relação ao que foi alterado. 
* As _Branchs_ e _issues_, além de todo o código, serão escritas em português.