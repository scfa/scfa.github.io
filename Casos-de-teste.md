### **Versão 1.0**

### Histórico da Revisão
Data|Versão|Descrição|Autor
-----|------|---------|-------
30/03/2016|1.0|Criação do documento| Jônnatas Lennon Lima Costa

* ###[UC01: Cadastrar Usuário](UC01---Criar-Usuario)

  * ####**CT001:** Cadastrar usuário com os campos preenchidos corretamente.
    **Descrição:** Este caso de teste tem por finalidade, testar se o sistema cadastra corretamente do usuário.

    **Pré-condições:** Campos preenchidos corretamente.

    **Pós-condições:** O sistema exibirá uma mensagem de sucesso no cadastro.

    **Dados requeridos:** [RN04](https://github.com/vitornere/partiuformar/wiki/Regras-de-Neg%C3%B3cio#2------------------defini%C3%A7%C3%B5es)

  * ####**CT002:** Cadastrar usuário com um campo obrigatório em branco.
    **Descrição:** Este caso de teste tem por finalidade, exibir uma mensagem de erro ao cadastrar um usuário com algum campo obrigatório em branco.

    **Pré-condições:** Campos preenchidos corretamente, com algum campo obrigatório em branco.

    **Pós-condições:** O sistema exibirá uma mensagem informando que o(s) campo(s) não pode ficar em branco.

    **Dados requeridos:** [RN04](https://github.com/vitornere/partiuformar/wiki/Regras-de-Neg%C3%B3cio#2------------------defini%C3%A7%C3%B5es)

  * ####**CT003:** Cadastrar usuário com um formato inválido na matrícula.
    **Descrição:** Este caso de teste tem por finalidade, exibir uma mensagem de erro ao cadastrar um usuário com a matrícula em formato inválido.

    **Pré-condições:** Campos preenchidos corretamente, com a matrícula em formato inválido.

    **Pós-condições:** O sistema exibirá uma mensagem informando erro no preenchimento da matrícula.

    **Dados requeridos:** [RN04](https://github.com/vitornere/partiuformar/wiki/Regras-de-Neg%C3%B3cio#2------------------defini%C3%A7%C3%B5es)

  * ####**CT004:** Cadastrar usuário com um formato inválido na senha.
    **Descrição:** Este caso de teste tem por finalidade, exibir uma mensagem de erro ao cadastrar um usuário com a senha em formato inválido.

    **Pré-condições:** Campos preenchidos corretamente, com a senha em formato inválido.

    **Pós-condições:** O sistema exibirá uma mensagem informando erro no preenchimento da senha.

    **Dados requeridos:** [RN04](https://github.com/vitornere/partiuformar/wiki/Regras-de-Neg%C3%B3cio#2------------------defini%C3%A7%C3%B5es)


  * ####**CT005:** Cadastrar usuário com um formato inválido no email.
    **Descrição:** Este caso de teste tem por finalidade, exibir uma mensagem de erro ao cadastrar um usuário com o email em formato inválido.

    **Pré-condições:** Campos preenchidos corretamente, com o email em formato inválido.

    **Pós-condições:** O sistema exibirá uma mensagem informando erro no preenchimento do email.

    **Dados requeridos:** [RN04](https://github.com/vitornere/partiuformar/wiki/Regras-de-Neg%C3%B3cio#2------------------defini%C3%A7%C3%B5es)

* ###[UC02: Editar Usuário](https://github.com/vitornere/partiuformar/wiki/Especifica%C3%A7%C3%A3o-do-Caso-de-Uso-UC02---Editar-Usu%C3%A1rio#uc02---editar-usu%C3%A1rio)

  * ####**CT006:**  Editar usuário com os campos corretamente.
    **Descrição:** Este caso de teste tem por finalidade, exibir uma mensagem de sucesso da operação, quando campos foram editados corretamente.

    **Pré-condições:** Campos editados corretamente.

    **Pós-condições:** O sistema exibirá uma mensagem informando sucesso na edição.

    **Dados requeridos:** [RN04](https://github.com/vitornere/partiuformar/wiki/Regras-de-Neg%C3%B3cio#2------------------defini%C3%A7%C3%B5es)

  * ####**CT007:**  Editar usuário mantendo alguns campos em branco.
    **Descrição:** Este caso de teste tem por finalidade, exibir uma mensagem de erro ao editar um usuário com algum campo obrigatório em branco.

    **Pré-condições:** Campos editados corretamente, mantendo algum campo obrigatório em branco.

    **Pós-condições:** O sistema exibirá uma mensagem, informando que o campo não pode permanecer em branco.

    **Dados requeridos:** [RN04](https://github.com/vitornere/partiuformar/wiki/Regras-de-Neg%C3%B3cio#2------------------defini%C3%A7%C3%B5es)


* ###[UC03: Consultar Usuário](https://github.com/vitornere/partiuformar/wiki/Especifica%C3%A7%C3%A3o-do-Caso-de-Uso-UC03---Consultar-Usu%C3%A1rio#uc03---consultar-usu%C3%A1rio)

  * ####**CT008:**  Consultar um usuário, com os campos preenchidos corretamente.
    **Descrição:** Este caso de teste tem por finalidade, verificar se o sistema executa a consulta de um usuário, com os campos da busca preenchidos corretamente. 

    **Pré-condições:** Campos preenchidos corretamente.

    **Pós-condições:** O sistema exibirá os dados do usuário.

    **Dados requeridos:** [RN04](https://github.com/vitornere/partiuformar/wiki/Regras-de-Neg%C3%B3cio#2------------------defini%C3%A7%C3%B5es)

  * ####**CT009:**  Consultar um usuário inexistente.
    **Descrição:** Este caso de teste tem por finalidade, verificar se o sistema envia uma mensagem quando consulta-se um usuário inexistente. 

    **Pré-condições:** Campos preenchidos corretamente na consulta de um usuário inexistente.

    **Pós-condições:** O sistema exibirá uma mensagem informando que o usuário não existe

    **Dados requeridos:** [RN04](https://github.com/vitornere/partiuformar/wiki/Regras-de-Neg%C3%B3cio#2------------------defini%C3%A7%C3%B5es)