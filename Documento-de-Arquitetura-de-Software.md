<h1>#PartiuFormar</h1>

## **Documento de Arquitetura de Software**

### **Versão 1.0**

### Histórico da Revisão
Data|Versão|Descrição|Autor
-----|------|---------|-------
27/03/2016|1.0|estruturação inicial do documento|Jônnatas Lennon Lima Costa
31/03/2016|1.1|Visão Geral, inicio Restrições|Eduardo Brasil 
### 1. Introdução         
#### 1.1 Finalidade    
Este artefato detalha a arquitetura utilizada no desenvolvimento do sistema <strong><em>#PartiuFormar</em></strong>. 

#### 1.2 Escopo 
Este documento trata da implementação arquitetura do #PartiuFormar com base nos diagramas <em>UML</em> acerca dos casos de uso, diagramas de classe, além da visão lógica do sistema com o detalhamento da arquitetura MVC utilizada, no desenvolvimento.

#### 1.3 Definições, Acrônimos e Abreviações     

#### 1.4 Referências     
[Documento de Arquitetura de Software (RUP)](http://www.wthreex.com/rup/process/artifact/ar_sadoc.htm)
[Diagrama de Casos de Uso](https://github.com/vitornere/partiuformar/wiki/Diagrama-de-Casos-de-Uso)

#### 1.5 Visão Geral 

O sistema **#PartiuFormar** é uma aplicação web construída de acordo com o modelo de arquitetura **MVC** (model-view-controller).

1. A camada de _Model_ representa os modelos de dados, os quais devem estar descritos pelas regras de negócio da aplicação, ou seja esta parte do sistema lida com os dados e as regras de negócio.

2. A camada de _View_ corresponde a parte gráfica, onde é apresentado para o usuário as informações de forma clara e compreensível, fazendo o uso de elementos de design para transmitir as informações de forma visualmente claras para o usuário.

3. A camada _Controller_ se trata da parte que processa cada ação do sistema, como por exemplo, requisições do usuário. Didaticamente, pode ser entendida como uma ponte de ligação entre a Model e a View, ou seja a _Controller_ interpreta os eventos que acontecem na camada View, e opera os dados que estão na _Model_, estabelecendo a comunicação com a _DAO_ a qual fica com a responsabilidade de armazenar estes dados no banco de dados da aplicação.

4. A camada _DAO_ (Data Access Object) é responsável, por manter a persistência no banco de dados, dos dados descritos pela Model.

5. Router esta camada é nativa do Rubi on Rails, a qual reconhece URLs e direciona a uma _Controller_ especifica.

### 2. Representação da Arquitetura
![Arquitetura](http://i.imgur.com/BxSbwTs.png)

Na representação acima tense o funcionamento da arquitetura MVC aplicada no rails, a qual segue os seguintes passos, usuário digita _http://exemplo.com/bem-vindo .

1. O _Browser_ faz uma solicitação para o _URL_ /bem-vindo, o pedido atinge o <em><strong>Rails router</strong></em>.
2. O _Router_ mapeia o URL para uma _Controller_, para a manipulação da solicitação.
3. A _Controller_ recebe o pedido, e pede a _Model_ buscar os dados no banco de dados na _DAO_.
4. O _Model_ retorna dados para a ação da _Controller_.
5. A _Controller_, passa os dados para a _View_.
6. A _View_ renderiza e retorna a página como HTML, de volta para o _Browser_.

![Visão geral](http://i.imgur.com/Hp4yBrN.png)

### 3. Restrições de Arquitetura e Metas 
A arquitetura definida:

O sistema deverá ser desenvolvido usando Ruby on Rails, que é uma framework escrito na linguagem Ruby e baseado no padrão de arquitetura MVC (Model-View-Controller), como já citado neste documento.

Para a persistência de dados será utilizado o SQLite3, devido a sua praticidade e estabilidade.

### 4. Visão de Casos de Uso

O caso de uso fundamental à arquitetura é:

>> [UC 001 – MANTER USUÁRIOS](https://github.com/vitornere/partiuformar/wiki/Especifica%C3%A7%C3%A3o-de-Caso-de-Uso:-Manter-Usu%C3%A1rio#especifica%C3%A7%C3%A3o-de-caso-de-uso-manter-usu%C3%A1rio)

![UC_Arquitetura](http://i.imgur.com/1onQ8e6.jpg)

#### 4.1 Realizações de Casos de Uso

Os [diagramas de sequência](https://github.com/vitornere/partiuformar/wiki/Diagramas-de-Sequ%C3%AAncia-de-Sistema) dos casos de uso, fornecem a visualização da comunicação entre as camadas.
 
### 5. Visão Lógica

O usuário interage com o sistema através da view, realizando alguma operação no sistema, a view solicita a controller a ação realizada, A controller processa as informações por meio da  comunicação com a model e a Dao, que por sua vez se comunica com o banco de dados, que por conseguinte repassa o resultado da operação solicitada para a view.

#### 5.1 Visão Geral    

A camada de View apenas deve conter classes responsáveis pela parte front-end parte da interação visual com o usuário. As classes da View se comunicam apenas com as da Controller, através de requisições.
 
#### 5.2 Pacotes de Design Significativos do Ponto de Vista da Arquitetura     

### 6. Visão de Processos

### 7. Visão de Implantação

### 8. Visão de Implementação
#### 8.1 Visão Geral     
#### 8.2 Camadas 
    
### 9. Visão de Dados 

#### 9.1 Modelo lógico
Diagrama de esquema do banco de dados, feito na ferramenta MySQL Workbench. 
![Lógico](http://i.imgur.com/wYyHD9Y.png)

### 10. Tamanho e Desempenho               

### 11. Qualidade   