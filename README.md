# Dashboard de Vendas

Este projeto é um dashboard de vendas interativo desenvolvido em Python usando a biblioteca Streamlit. O dashboard permite a visualização de diversos aspectos das vendas, incluindo receita e quantidade de vendas por região, mês, categoria e vendedor.

## Funcionalidades

- **Filtros Interativos**: O usuário pode filtrar os dados por região, ano e vendedores específicos.
- **Visualizações de Dados**: O dashboard inclui vários gráficos, como gráficos de barras, gráficos de linha e mapas de scatter geo, para representar a receita e a quantidade de vendas.
- **Dados em Tempo Real**: Os dados são obtidos a partir de uma API e transformados em um dataframe do Pandas.
- **Download de Dados**: Os dados são salvos em formato parquet para fácil manipulação e leitura.

## Tecnologias Utilizadas

- **Streamlit**: Para criação da interface do usuário e interatividade.
- **Requests**: Para fazer requisições HTTP e obter dados da API.
- **Pandas**: Para manipulação e análise de dados.
- **Plotly Express**: Para criação de gráficos interativos.

## Instalação

1. Clone este repositório:

   ```sh
   https://github.com/ingridcristh/dashboard_vendas_streamlit.git
   ```

2. Navegue até o diretório do projeto:

   ```sh
   cd nome_do_repositorio
   ```

3. Crie um ambiente virtual:

   ```sh
   python -m venv venv
   ```

4. Ative o ambiente virtual:

   - No Windows:

     ```sh
     venv\Scripts\activate
     ```

   - No macOS/Linux:

     ```sh
     source venv/bin/activate
     ```

5. Instale as dependências:

   ```sh
   pip install -r requirements.txt
   ```

## Uso

1. Execute o script Streamlit:

   ```sh
   streamlit run Dashboard.py
   ```

2. Acesse o dashboard através do navegador web no endereço:

   ```
   https://dashboard-vendasapp.streamlit.app
   ```

## Estrutura do Projeto

- **Dashboard.py**: Contém o código principal do dashboard.
- **requirements.txt**: Lista de dependências necessárias para rodar o projeto.
- **produtos.parquet**: Arquivo de dados salvo em formato parquet.
- **Dados brutos.py** : Contém os dados brutos obtido da [API](https://labdados.com/produtos) , onde é possível filtrados e baixar em formato csv

## Funcionalidades do Dashboard

### Filtros

- **Região**: Filtre os dados por uma das cinco regiões do Brasil ou selecione "Brasil" para visualizar dados de todas as regiões.
- **Ano**: Filtre os dados por um ano específico ou selecione "Dados de todo o período" para visualizar todos os anos.
- **Vendedores**: Selecione vendedores específicos para filtrar os dados.

### Abas

1. **Receita**:
   - Métrica de receita total.
   - Gráfico de mapa mostrando a receita por estado.
   - Gráfico de barras dos top estados em receita.
   - Gráfico de linha da receita mensal.
   - Gráfico de barras da receita por categoria.

2. **Quantidade de Vendas**:
   - Métrica de quantidade total de vendas.
   - Gráfico de mapa mostrando a quantidade de vendas por estado.
   - Gráfico de barras dos top estados em quantidade de vendas.
   - Gráfico de linha da quantidade de vendas mensal.
   - Gráfico de barras da quantidade de vendas por categoria.

3. **Vendedores**:
   - Input para selecionar a quantidade de top vendedores a serem exibidos.
   - Métrica de receita total.
   - Gráfico de barras dos top vendedores por receita.
   - Métrica de quantidade total de vendas.
   - Gráfico de barras dos top vendedores por quantidade de vendas.

## Contribuição

Contribuições são bem-vindas! Sinta-se à vontade para abrir uma issue ou enviar um pull request.

