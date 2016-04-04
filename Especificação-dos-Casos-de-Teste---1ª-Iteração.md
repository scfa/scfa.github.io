# **Especificação dos Casos de Teste - 1ª Iteração**

##  ***#PartiuFormar***

### **Versão 1.0**

### Histórico da Revisão
Data|Versão|Descrição|Autor
-----|------|---------|-------
03/04/2016|0.1|Caso de teste 01|Eduardo Brasil|

| Caso de testetradicional |          |        |
|--------------------------|----------|--------|
| ID                       |     UC  FA01     
| Nome                     |  Fluxo básico do caso de uso:  Cadastrar aluno
| Ambiente                 |    Mozilla Firefox v. 41.0      |        |
| Propósito                |  Verificar se os usuários estão sendo criados a partir de um formulário web.        |        |
| Pré Condições            |    Ter o Mozilla Firefox instalado e ter iniciado o servidor local      |        |
| Procedimentos            | Entradas | Saidas |
|           01               |       Abra o navegador Mozilla Firefox   |    O navegador deverá abrir já com acesso à internet    |
|            02              |     Acesse: http://localhost:3000/Usuarios     |    Devera ser exibido a página inicial do site.    |
|             03             |   Clique em novo usuario no menu principal.	       |     Deverá ser exibida uma lista de Itens para serem preenchidos   |
|              04            |      Preencha os campos necessários para criar um usuario, seguindo as orientações indicadas em campo.    |    Os dados devem permanecer inalterados quando o usuário selecionar outro campo    |
|              05            |    Clique em Criar Usuario      |  O sistema deve registrar o usuário no banco de dados e redirecionar o usuário para a página do mostrando o usuário  criado.      |
|              Pós Condição          |      Uma mensagem de sucesso deve ser exibida na aba superior, Os dados do evento devem ser exibidos na tela e o evento deve estar registrado no banco de dados da aplicação.   |    