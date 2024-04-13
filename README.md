# Controle de Gastos

Este projeto é um sistema de controle de gastos desenvolvido com HTML, JavaScript e Bootstrap. Ele permite o cadastro de gastos, listagem e visualização dos gastos por categoria e por dia, usando gráficos interativos para facilitar a análise dos dados.

## Funcionalidades

- **Cadastro de Gastos**: Permite o registro de novos gastos, incluindo a descrição, o valor, a data e a categoria.
- **Listagem de Gastos**: Exibe uma tabela com todos os gastos cadastrados, permitindo a edição e exclusão de registros.
- **Gastos por Categoria**: Exibe um gráfico de pizza mostrando a distribuição dos gastos por categoria.
- **Gastos por Dia**: Exibe um gráfico de barras mostrando a soma dos gastos por dia.

## Dependências

- [Bootstrap 4.3.1](https://getbootstrap.com/): Framework CSS para a interface do usuário.
- [jQuery 3.4.1](https://jquery.com/): Biblioteca JavaScript para facilitar a manipulação do DOM e eventos.
- [Chart.js 2.7.1](https://www.chartjs.org/): Biblioteca JavaScript para a criação de gráficos interativos.

## Como Usar

1. Clone o repositório para o seu computador.
2. Abra o arquivo `index.html` em um navegador web.
3. Você será apresentado à interface do controle de gastos.
4. Utilize as abas para navegar entre as diferentes funcionalidades:
    - **Cadastro**: Registre novos gastos.
    - **Gastos por Categoria**: Visualize os gastos por categoria em um gráfico de pizza.
    - **Gastos por Dia**: Visualize os gastos por dia em um gráfico de barras.

## Documentação do Código

### index.html

- A interface principal da aplicação é estruturada em abas (navegação por categoria) usando Bootstrap.
- Cada aba contém um formulário ou um gráfico, conforme a funcionalidade desejada.
- O formulário de cadastro está presente na aba "Cadastro".
- Os gráficos de gastos por categoria e por dia são exibidos nas abas "Gastos por categoria" e "Gastos por dia", respectivamente.

### scripts.js

- O código JavaScript gerencia as funcionalidades do projeto:
    - **Adicionar**: Função para adicionar um novo gasto ao localStorage.
    - **Editar**: Função para editar um gasto existente.
    - **Listar**: Função para listar os gastos cadastrados na tabela.
        - Calcula os totais de gastos por categoria e por dia para alimentar os gráficos.
    - **Excluir**: Função para excluir um gasto.
- O código também gerencia eventos de clique para edição e exclusão de gastos.
- Ao carregar a página, a função `Listar()` é chamada para exibir os dados existentes.
