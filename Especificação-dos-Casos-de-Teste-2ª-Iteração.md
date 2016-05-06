# **Especificação dos Casos de Teste 2ª Iteração**

### **Versão 1.0**

### Histórico da Revisão
Data|Versão|Descrição|Autor
-----|------|---------|-------
05/05/2016|1.0|Criação do documento| Eduardo Brasil Martins

* ###[UC05: Criar Disciplina](https://github.com/vitornere/partiuformar/wiki/UC05---Criar-Disciplina)

  * ####**CT001:** Cadastrar Disciplina com os campos preenchidos corretamente.
    **Descrição:** Este caso de teste tem por finalidade, testar se o sistema cadastra corretamente a disciplina.

    **Pré-condições:** Campos preenchidos corretamente.

    **Pós-condições:** O sistema exibirá uma mensagem de sucesso no cadastro.

    **Dados requeridos:** [RN05](https://github.com/vitornere/partiuformar/wiki/Regras-de-Neg%C3%B3cio#disciplinas)

  * ####**CT002:** Cadastrar disciplina com um campo obrigatório em branco.
    **Descrição:** Este caso de teste tem por finalidade, exibir uma mensagem de erro ao cadastrar uma disciplina com algum campo obrigatório em branco.

    **Pré-condições:** Campos preenchidos corretamente, com algum campo obrigatório em branco.

    **Pós-condições:** O sistema exibirá uma mensagem informando que o(s) campo(s) não pode ficar em branco.

    **Dados requeridos:** [[RN06](https://github.com/vitornere/partiuformar/wiki/Regras-de-Neg%C3%B3cio#disciplinas)]

  * ####**CT003:** Cadastrar disciplina com um código inválido.
    **Descrição:** Este caso de teste tem por finalidade, exibir uma mensagem de erro ao cadastrar uma disciplina com o código em formato inválido.

    **Pré-condições:** Campos preenchidos corretamente, com o código da disciplina em formato inválido.

    **Pós-condições:** O sistema exibirá uma mensagem informando erro no preenchimento do código da disciplina.

    **Dados requeridos:** [RN05](https://github.com/vitornere/partiuformar/wiki/Regras-de-Neg%C3%B3cio#disciplinas)


* ###[UC06: Editar Disciplina](https://github.com/vitornere/partiuformar/wiki/UC06---Editar-Disciplina)

  * ####**CT006:**  Editar disciplina com os campos corretamente.
    **Descrição:** Este caso de teste tem por finalidade, exibir uma mensagem de sucesso da operação, quando campos foram editados corretamente.

    **Pré-condições:** Campos editados corretamente.

    **Pós-condições:** O sistema exibirá uma mensagem informando sucesso na edição.

    **Dados requeridos:** [RN06](https://github.com/vitornere/partiuformar/wiki/UC06---Editar-Disciplina)

  * ####**CT007:**  Editar disciplina mantendo alguns campos em branco.
    **Descrição:** Este caso de teste tem por finalidade, exibir uma mensagem de erro ao editar uma disciplina com algum campo obrigatório em branco.

    **Pré-condições:** Campos editados corretamente, mantendo algum campo obrigatório em branco.

    **Pós-condições:** O sistema exibirá uma mensagem, informando que o campo não pode permanecer em branco.

    **Dados requeridos:** [RN06](https://github.com/vitornere/partiuformar/wiki/UC06---Editar-Disciplina)


* ###[UC07: Consultar Disciplina](https://github.com/vitornere/partiuformar/wiki/UC07---Consultar-Disciplina)

  * ####**CT008:**  Consultar uma disciplina, com os campos preenchidos corretamente.
    **Descrição:** Este caso de teste tem por finalidade, verificar se o sistema executa a consulta de uma disciplina, com os campos da busca preenchidos corretamente. 

    **Pré-condições:** Campos preenchidos corretamente.

    **Pós-condições:** O sistema exibirá os dados da disciplina.

    **Dados requeridos:** [RN06](https://github.com/vitornere/partiuformar/wiki/UC07---Consultar-Disciplina)

  * ####**CT009:**  Consultar uma disciplina inexistente.
    **Descrição:** Este caso de teste tem por finalidade, verificar se o sistema envia uma mensagem quando consulta-se uma disciplina inexistente. 

    **Pré-condições:** Campos preenchidos corretamente na consulta de uma disciplina inexistente.

    **Pós-condições:** O sistema exibirá uma mensagem informando que a disciplina não existe

    **Dados requeridos:** [RN06](https://github.com/vitornere/partiuformar/wiki/UC07---Consultar-Disciplina)

* ###[UC08: Excluir Disciplina](https://github.com/vitornere/partiuformar/wiki/UC08---Excluir-Disciplina)


  * ####**CT010:**  Excluir disciplina.
    **Descrição:** Este caso de teste tem por finalidade, verificar se o sistema está excluindo uma disciplina corretamente. 

    **Pré-condições:** Opção de exclusão do administrador esteja selecionada.

    **Pós-condições:** O sistema exibirá uma mensagem informando que a disciplina foi excluída com sucesso.
