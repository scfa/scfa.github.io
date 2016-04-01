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
#### 1.5 Visão Geral 

O sistema **#PartiuFormar** é uma aplicação web construída de acordo com o modelo de arquitetura **MVC** (model-view-controller).

1. A camada de _Model_ é parte do sistema que lida com os dados e as regras de negócio.

2. A camada de _View_ corresponde a parte gráfica, onde é apresentado para o usuário as informações de forma clara e compreensível, fazendo o uso de elementos de design para transmitir as informações de forma visualmente claras para o usuário.

3. A camada _Controller_ se trata da parte que processa cada ação do sistema, como por exemplo, requisições do usuário. Didaticamente, pode ser entendida como uma ponte de ligação entre a Model e a View.

4. A camada _DAO_ (Data Access Object) é responsável, por manter a persistência no banco de dados.

### 2. Representação da Arquitetura
![Arquitetura](http://i.imgur.com/BxSbwTs.png)

### 3. Restrições de Arquitetura e Metas 
A arquitetura definida 

#### 3.1 Restrições 

O sistema deverá ser desenvolvido usando Ruby on Rails, que é uma framework escrito na linguagem Ruby e baseado no padrão de arquitetura MVC (Model-View-Controller), como já citado neste documento.

Para a persistência de dados será utilizado o SQLite3, devido a sua praticidade e estabilidade.

### 4. Visão de Casos de Uso

O caso de uso fundamental à arquitetura é:

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

10. Tamanho e Desempenho               

11. Qualidade   
