1. Introdução

1.1. Finalidade

Este documento tem por finalidade manter o registro das decisões arquiteturais, das alternativas de solução, bem como das influências dos fatores.

2. Memória Técnica

2.1. Resumo da solução

Utilização do padrão Faca para garantir gerenciar o controle de acesso de modo dinâmico para os usuários e administradores no sistema.

2.2. Fatores

Gerencia o acesso a funcionalidades na gestão do sistema partiuformar, garantindo assim que cada integrante tenha acesso de acordo com as suas responsabilidades.

2.3. Solução

Utilizou-se de um padrão de projeto GoF da categoria estrutural denominado Façade. Criou-se então duas classes a admin_facade e student_facade.

Estas classes utilizam a classe authenticate para verificar o nível de acesso de usuário e através do facade redireciona os usuários para as respectivas funcionalidades associadas ao mesmo, com o admin podendo cadastrar e excluir disciplinas e o os estudantes somente com acesso para visualização das mesmas.

E para o student_facade, tem-se as responsabilidades no gerenciamento da grade curricular e o fluxo do mesmo.

2.4. Motivação
Houve a necessidade de separara as responsabilidades dos usuários por nível de acesso, sem auterar as classes de disciplinas, grade e fluxo.

2.5. Pendências

Não se aplica.

2.6. Alternativas

Poderia-se criar esta verificação na classe authenticate, porém a classe acabaria ficando muito grande, diminuindo a coesão e aumentando o acoplamento desta classe