# 1. Introdução

## 1.1. Finalidade

Este documento tem por finalidade manter o registro das decisões arquiteturais tomadas dobre a aplicação do padrão Strategy no calculo do IRA, das alternativas de solução, bem como das influências dos fatores.

# 2. Memória Técnica

## 2.1. Resumo da solução

Utilização do padrão Strategy para o calculo do IRA de um aluno, de modo dinâmico sem alterar as classe a qual ele opera, encapsulando os algoritmos para o calculo do IRA em classes especificas.

## 2.2. Fatores

Necessitou-se de alternar os algorítimos para o calculo do irar entre as classes encapsulando os mesmos, evitando assim códigos repetidos no sistema, uma troca fluida entre os algoritmos de calculo do ira quando necessário.

## 2.3. Solução

Aplicou-se o padrão Strategy para realizar a troca de algoritmos, assim definindo estratégias diferentes para o calculo do ira com base na menção do aluno.

Deste modo, criou-se as seguintes classes ira_abstract, que terá um templete para as subclasses do calculo do IRA, e as classes ira_sr, ira_ii, ira_mi, ira_mm, ira_ms, ira_ss, além da classe ira_tr.

## 2.4. Motivação

Para evitar problemas de código duplicado e uma série de verificações, além de facilitar a manutenção do código, utilizou-se o padrão strategy, garantindo esta alternância entre os algoritmos.

## 2.5. Pendências

Não se aplica.

## 2.6. Alternativas

Acreditamos que o strategy seja o algoritmo que melhor se encaixa neste projeto.