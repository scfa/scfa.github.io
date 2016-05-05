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




