**#PartiuFormar**
**Especificações Suplementares**
 
**Versão 1.0**

### Histórico da Revisão
Data|Versão|Descrição|Autor
-----|------|---------|-------
24/03/2015|1.0|Iniciação|Jônnatas Lennon

#### 1. Introdução

##### 1.1 Finalidade
Este artefato consiste na descrição dos requisitos não funcionais do sistema **#PartiuFormar**, os quais podem servir futuramente nas fases de teste, a qual verifica a compatibilidade do **#PartiuFormar** com os RNF descritos, além deste artefato ser utilizado na fase de desenvolvimento, a qual junto aos Requisitos Funcionais as especificadões suplementares servem para completar os requisitos do sistema. 

##### 1.2 Escopo
O **#PartiuFormar** será um sistema que auxiliará o graduando em uma Universidade de Ensino Superior a organizar de modo mais eficiente o seu semestre, além do fluxo durante o curso do mesmo.

##### 1.3 Definições, Acrônimos e Abreviações
Vide documento visão.

##### 1.4 Referências

##### 1.5 Visão Geral
Inicialmente este artefato apresenta, uma introdução sobre o projeto, para o conhecimento do problema. Seguindo, há a distribuição dos requisitos suplementares em funcionalidade, usabilidade, confiabilidade, desempenho, suportabilidade, restrições de design, requisitos de sistemas, de ajuda e de documentação de usuário _online_, interfaces, requisitos de licenciamento, observações legais de Copyright e outras e padrões aplicáveis.

#### 2. Funcionalidade

##### 2.1 Tratamento de erros
* **RNF 01** - O sistema deve ser resiliente (capaz de se recuperar a erros), retornando à configuração anterior ao erro.

##### 2.2 Segurança
* **RNF 02** - As funcionalidades que só podem ser acessadas pelo administrador do sistema devem exigir a autenticação necessária.


#### 3. Usabilidade

##### 3.1 Apreensibilidade (capacidade de aprender a utilizar o sistema)
* **RNF 03** - Usuário comum necessitará de pelo menos 20 minutos para aprender as funcionalidades do **#PartiuFormar**.
* **RNF 04** - Usuários mais experientes necessitarão de 10 minutos para aprenderem as funcionalidades do **#PartiuFormar**.  
* **RNF 05** - O Usuário comum conseguirá realizar uma das operações básicas de cadastro, consulta, ou exclusão em pelo menos 2 minutos, ao primeiro uso.

##### 3.2 Operacionalidade
* **RNF 06** - Deve-se evitar abrir janelas _pop-ups_ no **#PartiuFormar**.

##### 3.3 Inteligibilidade
* **RNF 07** - As paginas do **#PartiuFormar** devem ser claras e simples.
* **RNF 08** - A informação deve estar disposta de modo intuitivo e lógico, mantendo a padronização dos menus e links disponíveis em todas as páginas. 
* **RNF 09** - Elementos visuais presentes em todas as páginas, como por exemplo logotipos, atalhos e caixas de busca, devem manter-se no mesmo lugar.
* **RNF 10** - Deve-se disponibilizar uma ferramenta de busca em todas as páginas.

#### 4. Confiabilidade
* **RNF 11** - O sistema deve está disponível no dia 24 de Julho de 2016.

#### 5. Segurança
* **RNF 12** - Em caso de exclusão de algum item, o sistema sempre deve exibir uma mensagem pedindo a confirmação.
* **RNF 13** - O Sistema deve exigir que o usuário execute o _login_ na aplicação, e exiba um ícone confirmando o _login_ em todas as telas.
* **RNF 14** - As ações no **#PartiuFormar** devem ser reversíveis.
* **RNF 15** - As mensagens de erro devem ser claras.

#### 6. Desempenho
* ** RNF 16** - O sistema não pode exceder 2 segundos ao realizar uma tarefa básica, como excluir, cadastrar, consultar e alterar.

#### 7. Suportabilidade
* **RNF 17** - O sistema deve funcionar em qualquer navegador com suporte a HTML5, como _Chrome_ 17 ou superior.

#### 8. Restrições de Design
* **RNF 18** - A arquitetura deve respeitar o padrão MVC (_model-view-controller_).
* **RNF 19** - O sistema deve obedecer os padrões definidos na orientação a objetos.
* **RNF 20** - O sistema deve obedecer as convenções estabelecidas no _Ruby on Rails_ 4.
* **RNF 21** - O sistema deve obedecer os padrões definidos em HTML 5, CSS 3 e _javascript_.

#### 9. Requisitos de Sistema de Ajuda e de Documentação de Usuário On-line
* **RNF 22 -** Deve-se criar uma _Wiki_ contendo todas as informações do projeto.

#### 10. Requisitos de Licenciamento
* **RNF 23** - O sistema deve ser desenvolvido em código aberto.