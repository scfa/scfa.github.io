<h1>#PartiuFormar</h1>

## **Documento de Arquitetura de Software**

### **Versão 1.6**

### Histórico da Revisão
Data|Versão|Descrição|Autor
-----|------|---------|-------
27/03/2016|1.0|Estruturação inicial do documento|Jônnatas Lennon Lima Costa
31/03/2016|1.1|Visão Geral, inicio Restrições|Eduardo Brasil 
02/04/2016|1.2|Adição da seção 5.2|Vitor Nere
03/04/2016|1.3|Tamanho e Desempenho ,Qualidade|Eduardo Brasil
03/04/2016|1.4|Adições e alterações das seções 5.1, 7.1, 8.1|Jônnatas Lennon
03/04/2016|1.5|Adição da seção 1.4 e ajustes|Vitor Nere
03/04/2016|1.6| Revisão do documento|Hugo Martins

### 1. Introdução         
#### 1.1 Finalidade    
Este artefato detalha a arquitetura utilizada no desenvolvimento do sistema <strong><em>#PartiuFormar</em></strong>. 

#### 1.2 Escopo 
Este documento trata da implementação arquitetura do #PartiuFormar com base nos diagramas <em>UML</em> acerca dos casos de uso, diagramas de classe, além da visão lógica do sistema com o detalhamento da arquitetura MVC utilizada, no desenvolvimento.  

#### 1.3 Referências     
[Documento de Arquitetura de Software (RUP)](http://www.wthreex.com/rup/process/artifact/ar_sadoc.htm)

[Diagrama de Casos de Uso](https://github.com/vitornere/partiuformar/wiki/Diagrama-de-Casos-de-Uso)

#### 1.4 Visão Geral 

Esse documento está dividido nas seguintes seções: 

1. Introdução
2. Representação da Arquitetura
3. Restrição de Arquitetura e Metas 
4. Visão de Casos de Uso
5. Visão Lógica
6. Visão de Implementação
7. Visão de Dados
8. Tamanho e Desempenho
9. Qualidade

### 2. Representação da Arquitetura

MVC padrão do Rails
![Arquitetura](http://i.imgur.com/BxSbwTs.png)

Na representação acima mostra o funcionamento da arquitetura MVC aplicada no _rails_, a qual segue os seguintes passos, usuário digita _http://exemplo.com/bem-vindo .

1. O _Browser_ faz uma solicitação para o _URL_ /bem-vindo, o pedido atinge o <em><strong>Rails router</strong></em>.
2. O _Router_ mapeia o URL para uma _Controller_, para a manipulação da solicitação.
3. O _Model_ retorna dados para a ação da _Controller_.
5. A _Controller_, passa os dados para a _View_.
6. A _View_ renderiza e retorna a página como HTML, de volta para o _Browser_.

### 3. Restrições de Arquitetura e Metas 
A arquitetura definida:

O sistema deverá ser desenvolvido usando _Ruby on Rails_, que é uma _framework_ escrito na linguagem _Ruby_ e baseado no padrão de arquitetura MVC (_Model-View-Controller_), como já citado neste documento.

Para a persistência de dados será utilizado o SQLite3, devido a sua praticidade e estabilidade.

### 4. Visão de Casos de Uso

O caso de uso fundamental à arquitetura é:

>> [UC 001 – MANTER USUÁRIOS](https://github.com/vitornere/partiuformar/wiki/Especifica%C3%A7%C3%A3o-de-Caso-de-Uso:-Manter-Usu%C3%A1rio#especifica%C3%A7%C3%A3o-de-caso-de-uso-manter-usu%C3%A1rio)

![UC_Arquitetura](http://i.imgur.com/1onQ8e6.jpg)

#### 4.1 Realizações de Casos de Uso

Os [diagramas de sequência](https://github.com/vitornere/partiuformar/wiki/Diagramas-de-Sequ%C3%AAncia-de-Sistema) dos casos de uso, fornecem a visualização da comunicação entre as camadas.
 
### 5. Visão Lógica

O usuário interage com o sistema através da _view_, realizando alguma operação no sistema, a _view_ solicita a _controller_ a ação realizada, A _controller_ processa as informações por meio da  comunicação com a _model_ e o datavase, que por sua vez se comunica com o banco de dados, que por conseguinte repassa o resultado da operação solicitada para a _view_.

#### 5.1 Visão Geral    

Visão geral da arquitetura
![Visão geral](http://i.imgur.com/Hp4yBrN.png)

O sistema **#PartiuFormar** é uma aplicação web construída de acordo com o modelo de arquitetura **MVC** (_model-view-controller_).

1. A camada de _View_ é responsável pelo front-end, onde é estabelecida a comunicação entre o usuário e a aplicação. A comunicação acontece apenas com a _Controlle_r, através de requisições.

2. A camada _Controller_ trata da parte que processa cada ação do sistema, como por exemplo, requisições do usuário. Didaticamente, pode ser entendida como uma ponte de ligação entre a _Model_ e a_ View_, ou seja a _Controller_ interpreta os eventos que acontecem na camada _View_, e opera os dados que estão na _Model_ validando os mesmos, estabelecendo a comunicação com o database a qual fica com a responsabilidade de armazenar estes dados no banco de dados da aplicação.

2. A camada de _Model_ representa os dados da aplicação, basicamente na camada _Model_ ocorre o tratamento da escrita, validação e leitura dos dados. Estes dados devem estar descritos pelas regras de negócio do sistema. Assim a _Model_, armazena se necessário os dados no database, e se comunica com a _Controller_ quando houver necessidade de exibição, e a _Controller_ decidirar em qual view exibir os dados da _Model_ .

4. Router esta camada é nativa do _Rubi on Rails_, a qual reconhece URLs e direciona a uma _Controller_ especifica.
 
![Imgur](http://i.imgur.com/86NTVFj.png)
Representação da visão geral do PartiuFormar

#### 5.2 Pacotes de Design Significativos do Ponto de Vista da Arquitetura     

Aqui encontra-se uma representação visual dos pacotes presentes neste projeto:

![](http://i.imgur.com/2cmoh2R.png)

### 6. Visão de Implementação
#### 6.1 Model
Como pode ser observado no diagrama abaixo, utilizamos o padrão **Strategy** para o calculo do **IRA**, isto ocorreu para dar maior flexibilidade ao código, este **Strategy** será aplicada na Grade curricular ao final do semestre, deste modo ao final do semestre em cada disciplina associada a grade aplica-se uma estrategia diferente para o calculo do ira com base na menção referente.

Utilizou-se também o padrão **State** para alternar os estados das menções referentes as disciplinas, assim uma disciplina pode ter 8 estados diferentes (cursando CC, trancamento TR, SR, II, MI, MM, MS, SS).

Para armazenar no fluxo as grades de semestres anteriores utilizou-se o padrão **Memento**, através deste padrão temos salvo as grades anteriores, para o calculo de um novo fluxo. 

Tem-se também o **facade** para controlar o acesso do usuário no sistema, assim para um estudante apenas algumas funcionalidades serão exibidas, já na fachada do administrador todas as funcionalidades serão exibidas, para organizar melhor estas classes, criou-se dois pacotes diferentes o _StudentInterface _e o _AdminInterface_. 

Representação do Diagrama de classes da _Model_. 

![Imgur](http://i.imgur.com/znyBaKa.png)

Admin Iterface package
![Imgur](http://i.imgur.com/JsAySpp.png)

Student Interface package
![Imgur](http://i.imgur.com/17AAXoD.png)

#### 6.2 View
As views são separadas em pastas, nestas pastas contem-se os arquivos utilizados para a renderização da views.
![Imgur](http://i.imgur.com/qZtiAjq.png)

#### 6.3 Controller
As controllers surgem por demanda, a medida que as classes de model são criadas, as classes de controller como o próprio nome diz funcionam como controladoras das requisições da View sobre os dados das models.
![Imgur](http://i.imgur.com/9jXgzbg.png)

### 7. Visão de Dados 

#### 7.1 Modelo Lógico
Diagrama de esquema do banco de dados, feito na ferramenta _MySQL Workbench_. 
![Lógico](http://i.imgur.com/TQHaqgl.png)         

#### 8. Visão de implantação
Para a implantação do partiuformar pode-se utilizar o Heroku, este é bem simples e facil de configurar.
![Imgur](http://i.imgur.com/PNAFUeB.png)

### 9. Tamanho e Desempenho               

O objetivo do **#PartirFormar** é fazer com que o máximo de usuários consigam acessar o app no menor tempo possível. todavia, os fatores de desempenho dependem do servidor em que o app esteja hospedado

### 10. Qualidade   

Com a definição da arquitetura, houve uma independência proporcionada ao dividir em três partes principais a aplicação. O MVC também torna mais simples a manutenção do software, pois sua estrutura de arquivos torna fácil localizar trechos específicos de código, esse padrão arquitetural é a melhor solução para o modelo de aplicações web que propomos.