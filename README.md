# Análise de Risco de Crédito - Análise Exploratória de Dados

Este projeto realiza uma Análise Exploratória de Dados (EDA) em um conjunto de dados de solicitações de crédito, com o objetivo de entender o perfil dos solicitantes. A análise foca em características demográficas, financeiras e sociais para extrair insights iniciais.

## 📁 Estrutura do Projeto

* `/data`: Contém os conjuntos de dados brutos.
    * `application_test.csv`: Dados de teste com informações sobre os solicitantes.
    * `application_train.csv`: (Ainda não incluído) Dados de treino que contêm a variável alvo (`TARGET`) indicando se um cliente pagou ou não o empréstimo.
* `/visualizations`: Armazena os gráficos gerados durante a análise.
* `Analise_Exploratoria.ipynb`: Notebook Jupyter com todo o passo a passo da análise, desde o carregamento dos dados até a geração dos gráficos e conclusões.
* `requirements.txt`: Lista de dependências Python para reproduzir o ambiente de análise.

## 📊 Análise Realizada

A análise atual, contida no notebook `Analise_Exploratoria.ipynb`, foca exclusivamente no conjunto de dados de teste e inclui:

1.  **Carregamento e Limpeza Inicial:** Leitura dos dados e verificação da integridade.
2.  **Estatísticas Descritivas:** Resumo estatístico das variáveis numéricas.
3.  **Visualização de Dados:**
    * Distribuição da Renda dos solicitantes.
    * Contagem dos diferentes Tipos de Renda.
    * Distribuição do Nível de Escolaridade.

## 🚀 Como Executar o Projeto

1.  **Clone este repositório:**
    ```bash
    git clone https://github.com/JoelsonAD/analise_risco_credito.git
    cd analise_risco_credito
    ```

2.  **Crie um ambiente virtual (recomendado):**
    ```bash
    python -m venv venv
    source venv/bin/activate  # No Windows: venv\Scripts\activate
    ```

3.  **Instale as dependências:**
    ```bash
    pip install -r requirements.txt
    ```

4.  **Execute o Jupyter Notebook:**
    ```bash
    jupyter notebook Analise_Exploratoria.ipynb
    ```

## ⏭️ Próximos Passos

* [ ] **Incluir `application_train.csv`**: Adicionar o dataset de treino para permitir a construção de um modelo preditivo.
* [ ] **Tratamento de Dados Faltantes**: Implementar estratégias para lidar com os valores nulos.
* [ ] **Engenharia de Features**: Criar novas variáveis a partir das existentes para melhorar o desempenho do modelo.
* [ ] **Treinamento de Modelo**: Construir e treinar um modelo de classificação (ex: Logistic Regression, LightGBM) para prever o risco de inadimplência.
* [ ] **Avaliação do Modelo**: Medir a performance do modelo utilizando métricas apropriadas como AUC-ROC.
