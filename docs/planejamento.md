# Planejamento do Projeto — Controle de Despesas Pessoais


## 1. Definição do problema

A falta de controle e organização das despesas pessoais dificulta o acompanhamento dos gastos, impedindo que o indivíduo
saiba quanto dinheiro está gastando, onde está gastando e quais categorias consomem a maior parte de seu orçamento.

Sem um registro organizado, torna-se mais difícil identificar hábitos de consumo, acompanhar os gastos ao longo do tempo
e tomar decisões financeiras conscientes.


## 2. Objetivo do projeto

Desenvolver uma aplicação de linha de comando (CLI), utilizando Python, que permita ao usuário gerenciar suas despesas
pessoais por meio do registro, edição, consulta e exclusão de despesas.

A aplicação deverá permitir a criação, edição e organização de categorias para classificar os gastos e facilitar sua 
consulta.

O sistema deverá apresentar resumos dos valores gastos em diferentes períodos: diário, semanal, mensal e anual, além de 
permitir consultas por categoria.

As operações de exclusão deverão solicitar confirmação do usuário, especialmente quando envolverem a remoção de uma
categoria e todas as despesas vinculadas a ela.

Os dados cadastrados deverão permanecer armazenados mesmo após o encerramento do programa.


## 3. Requisitos funcionais

RF01: Permitir a criação de categorias.

RF02: Permitir o registro de despesas.

RF03: Permitir a edição de despesas cadastradas.

RF04: Permitir a exclusão de despesas cadastradas.

RF05: Permitir a consulta de despesas cadastradas individualmente ou por meio de filtros de categoria e período.

RF06: Permitir a consulta do total gasto por categoria.

RF07: Permitir a consulta de despesas cadastradas em determinado período.

RF08: Permitir a edição de categorias cadastradas.

RF09: Permitir a exclusão de categorias, mediante confirmação do usuário. A exclusão de uma categoria deverá remover 
também todas as despesas associadas a ela.

RF10: Permitir a consulta do total de despesas em períodos diários, semanais, mensais e anuais.

RF11: Permitir o armazenamento persistente das despesas e categorias cadastradas, mantendo os dados disponíveis após o 
encerramento do programa.

## 4. Requisitos não funcionais

RNF01: O sistema deverá validar os dados informados pelo usuário, impedindo o cadastro de informações inválidas.

RNF02: O sistema deverá apresentar mensagens claras e compreensíveis para orientar o usuário durante sua utilização.

RNF03: O sistema deverá tratar erros de entrada, permitindo que o usuário corrija informações inválidas sem provocar o 
encerramento inesperado do programa.

RNF04: O sistema deverá possuir uma interface de linha de comando (CLI) simples, organizada e de fácil utilização.

RNF05: O sistema deverá garantir a integridade dos dados armazenados, evitando alterações ou exclusões indevidas durante
as operações de gerenciamento.

RNF06: O sistema deverá manter uma organização interna que facilite a manutenção, a compreensão e a expansão do código.

RNF07: O sistema deverá funcionar utilizando recursos nativos do Python, sem exigir bibliotecas externas para suas 
funcionalidades principais.

RNF08: O sistema deverá armazenar os dados em arquivos locais, garantindo sua persistência entre diferentes execuções.


## 5. Regras de negócio

RN01: Toda despesa deverá estar associada a uma categoria previamente cadastrada.

RN02: O valor de uma despesa deverá ser maior que zero.

RN03: Cada despesa deverá possuir um identificador único.

RN04: Cada categoria deverá possuir um identificador único.

RN05: A exclusão de uma categoria deverá remover todas as despesas associadas a ela, após confirmação explícita do 
usuário.

RN06: O sistema não deverá permitir o cadastro de categorias com nomes duplicados.

RN07: O sistema deverá permitir a consulta das despesas cadastradas sem exigir a inclusão de novas informações.

RN08: Toda despesa deverá possuir, no mínimo, uma descrição, um valor, uma categoria e uma data.

RN09: As datas das despesas deverão ser armazenadas e utilizadas para realizar consultas e calcular os resumos por 
período.

RN10: A edição de uma categoria deverá atualizar o nome da categoria sem perder a associação com as despesas existentes.

## 6. Escopo da primeira versão

A primeira versão do projeto contemplará:

- Aplicação executada pelo terminal.
- Cadastro, edição, consulta e exclusão de categorias.
- Cadastro, edição, consulta e exclusão de despesas.
- Filtros de consulta por categoria e período.
- Cálculo de totais por categoria.
- Resumos financeiros diários, semanais, mensais e anuais.
- Armazenamento persistente utilizando arquivos JSON.
- Validação de dados e tratamento de erros.
- Utilização de recursos nativos do Python.

### Funcionalidades fora do escopo inicial

Não serão implementadas na primeira versão:

- Interface gráfica.
- Aplicativo para dispositivos móveis.
- Integração com bancos ou instituições financeiras.
- Sincronização de dados em nuvem.
- Cadastro de múltiplos usuários.
- Autenticação e controle de acesso.

Essas funcionalidades poderão ser consideradas em versões futuras.

## 7. Tecnologias e ferramentas

**Linguagem de programação:** Python 3.

**Interface:** Linha de comando (CLI).

**Armazenamento:** Arquivos JSON.

**Controle de versão:** Git.

**Hospedagem do código:** GitHub.

**Ambiente de desenvolvimento:** PyCharm.

## 8. Critérios de conclusão

O projeto será considerado concluído quando:

1. Todas as funcionalidades previstas nos requisitos funcionais estiverem implementadas.
2. O sistema validar corretamente os dados informados.
3. As operações de cadastro, edição, consulta e exclusão funcionarem corretamente.
4. Os resumos financeiros apresentarem resultados coerentes com os registros cadastrados.
5. Os dados permanecerem disponíveis após o encerramento e a reabertura do programa.
6. As operações críticas de exclusão solicitarem confirmação.
7. O código estiver organizado e documentado.
8. O projeto possuir testes básicos e documentação de utilização.
9. O código estiver versionado e publicado no GitHub.