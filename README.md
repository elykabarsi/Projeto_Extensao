# Análise de Dados de Aluguel de Impressoras

Este projeto realiza uma análise exploratória de dados de uma empresa que aluga impressoras. O objetivo é extrair insights sobre os contratos de aluguel, os tipos de impressoras mais populares, a distribuição dos clientes e a situação do inventário de impressoras.

## 📜 Descrição do Projeto

O projeto utiliza um conjunto de dados distribuído em quatro arquivos CSV: `Aluguel.csv`, `Aluguel2.csv`, `Impressora.csv` e `PessoaJuridica.csv`. A análise é conduzida em um Jupyter Notebook (`Projeto_Extensao.ipynb`) e utiliza bibliotecas de Python como Pandas, Matplotlib e Seaborn para manipulação, análise e visualização dos dados.

## 📊 Conjunto de Dados

O conjunto de dados é composto pelos seguintes arquivos:

*   **`Aluguel.csv` e `Aluguel2.csv`**: Contêm informações sobre os contratos de aluguel, incluindo:
    *   `ID`: Identificador único do aluguel.
    *   `ID_Cliente`: Identificador do cliente.
    *   `ID_Tipo_de_impressora`: Modelo da impressora alugada.
    *   `Duracao_em_meses`: Duração do contrato em meses.
    *   `Valor_Total`: Valor total do contrato.

*   **`Impressora.csv`**: Contém informações sobre as impressoras, como:
    *   `ID`: Identificador único da impressora.
    *   `ID_Tipo_de_impressora`: Modelo da impressora.
    *   `Ultima_manutencao`: Data da última manutenção.
    *   `Data_de_aquisicao`: Data de aquisição da impressora.
    *   `Disponibilidade`: Se a impressora está disponível para aluguel.
    *   `Em_uso`: Se a impressora está atualmente em uso.
    *   `Possui_defeito`: Se a impressora possui algum defeito.

*   **`PessoaJuridica.csv`**: Contém informações sobre os clientes (pessoas jurídicas), incluindo:
    *   `ID`: Identificador único do cliente.
    *   `Nome`: Nome da empresa cliente.
    *   `Endereco`: Endereço da empresa.
    *   `Telefone`: Telefone de contato.
    *   `Data_de_cadastro`: Data de cadastro do cliente.
    *   `CNPJ`: Cadastro Nacional da Pessoa Jurídica.
    *   `Porte`: Porte da empresa (ME, EPP, etc.).

## 📈 Análise Realizada

A análise de dados no Jupyter Notebook (`Projeto_Extensao.ipynb`) aborda os seguintes pontos:

1.  **Carregamento e Limpeza dos Dados**: Os dados dos arquivos CSV são carregados em DataFrames do Pandas.
2.  **Tratamento de Dados**:
    *   Aplicação de descontos no valor total dos aluguéis com base na duração do contrato.
    *   Ajuste de preço para um modelo de impressora específico.
3.  **Visualização de Dados**:
    *   **Distribuição da Duração dos Contratos**: Gráfico de barras mostrando a quantidade de contratos por duração (em meses).
    *   **Contagem Comparativa de Aluguéis**: Gráfico de barras comparando o número de aluguéis por modelo de impressora e duração do contrato.
    *   **Impressoras com Defeito**: Gráfico de barras mostrando a quantidade de impressoras com e sem defeito.
    *   **Disponibilidade das Impressoras**: Gráfico de barras mostrando a disponibilidade das impressoras no inventário.
    *   **Distribuição do Porte dos Clientes**: Gráfico de barras mostrando a distribuição do porte das empresas clientes.
    *   **Nuvem de Palavras**: Uma nuvem de palavras para visualizar os modelos de impressora mais frequentemente alugados.

## 🛠️ Tecnologias Utilizadas

*   **Python**: Linguagem de programação principal.
*   **Pandas**: Para manipulação e análise de dados.
*   **Matplotlib**: Para a criação de gráficos e visualizações.
*   **Seaborn**: Para a criação de visualizações estatísticas mais atraentes.
*   **WordCloud**: Para a criação da nuvem de palavras.
*   **Jupyter Notebook**: Ambiente interativo para a execução da análise.

## 🚀 Como Executar o Projeto

1.  **Clone o repositório:**
    ```bash
    git clone <url-do-repositorio>
    ```
2.  **Instale as dependências:**
    ```bash
    pip install pandas matplotlib seaborn wordcloud
    ```
3.  **Execute o Jupyter Notebook:**
    ```bash
    jupyter notebook Projeto_Extensao.ipynb
    ```