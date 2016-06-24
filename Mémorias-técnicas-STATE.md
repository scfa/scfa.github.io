# 1. Introdução

## 1.1. Finalidade

Este documento tem por finalidade manter o registro das decisões arquiteturais, das alternativas de solução, bem como das influências dos fatores.

# 2. Memória Técnica

## 2.1. Resumo da solução

Utilização do padrão State para manter o estado das menções do aluno das disciplinas em uma grade curricular.

## 2.2. Fatores

Organizar os diversos estados que uma disciplina possa ter em uma grade curricular, de modo dinamico. 

## 2.3. Solução

Utilizou-se de um padrão de projeto GoF da categoria comportamental denominado State. Criou-se então uma classe state_discipline, e as suas subclasses que variam os estados, sendo elas SR, II, MI, MM, MS, SS e TR.

Assim o aluno pode ter na sua grade curricular as disciplinas com estes estados variando ao longo do curso.

## 2.4. Motivação
Houve a necessidade de colocar de modo dinâmico a alteração destes estados de modo que quando uma nova menção seja inserida no sistema essa troca seja fluida com pouco esforço de manutenção.

## 2.5. Pendências

Não se aplica.

## 2.6. Alternativas
Poderia-se setar diretamente na instancia da disciplina o seu estado porém isto não teria o efeito desejado pela equipe.