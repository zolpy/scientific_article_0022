<!-- Tab simulation using details -->
<details open>
<summary>🇧🇷 Português</summary>

# Artigo Científico – Análise Preditiva da Severidade de Doenças em Cana-de-Açúcar

Este repositório contém o conjunto de dados sintéticos e o código-fonte (notebooks Jupyter) utilizados nas análises apresentadas no artigo científico: **"Análise Preditiva da Severidade da Podridão Vermelha em Cana-de-Açúcar Utilizando Dados Sintéticos e Modelos de Regressão Interpretáveis"**.

O objetivo deste projeto é demonstrar a viabilidade da aplicação de técnicas de Machine Learning para prever a severidade de sintomas de doenças em cana-de-açúcar, utilizando uma base de dados sintética e robusta, fundamentada em um estudo de referência sobre a patogenicidade de fungos dos gêneros *Colletotrichum* e *Fusarium*.

## 🎯 Objetivo do Repositório

Este repositório visa garantir a **reprodutibilidade completa** dos experimentos e análises descritos no artigo científico associado. Ele permite a exploração, validação ou adaptação dos modelos preditivos para a severidade da doença no colmo e as dimensões das lesões foliares. Serve como um recurso para pesquisadores interessados na aplicação de aprendizado de máquina à fitopatologia e agronomia de precisão, particularmente utilizando conjuntos de dados sintéticos.

## 📁 Estrutura do Repositório

-   **`/data/`**: Contém a base de dados sintética.
    -   📄 `dados_sinteticos_cana.xlsx`: Dataset com 10.000 registros, simulando ensaios de inoculação de diferentes espécies de fungos em cana-de-açúcar, com suas respectivas variáveis de entrada (tipo de inoculação, variedade) e de saída (severidade, comprimento e largura da lesão).
-   **`/notebooks/`**: Contém os notebooks Jupyter com todo o fluxo de análise.
    -   📄 `01_geracao_dados_sinteticos.ipynb`: Código para a geração da base de dados sintética com base nos parâmetros estatísticos do estudo de referência.
    -   📄 `02_analise_exploratoria_e_selecao_features.ipynb`: Análise exploratória dos dados (Box Plots, Matrizes de Correlação) e seleção de variáveis com base na importância de features do Random Forest.
    -   📄 `03_benchmark_modelos_regressao.ipynb`: Treinamento e avaliação de mais de 20 modelos de regressão para prever a severidade da doença e os sintomas foliares, utilizando validação cruzada.
    -   📄 `04_interpretabilidade_modelos_com_xai.ipynb`: Análise de interpretabilidade (XAI) do melhor modelo preditivo para severidade utilizando as bibliotecas SHAP e a análise de Dependência Parcial (PDP).
    -   📄 `05_previsao_em_novos_cenarios.ipynb`: Código final que utiliza os melhores modelos treinados para fazer previsões em um conjunto de novos cenários hipotéticos.
-   **`/figures/`**: Contém as visualizações geradas pelos notebooks.
    -   📄 `boxplot_severidade_por_especie.png`: Box plot da distribuição da severidade da doença por espécie de fungo.
    -   📄 `feature_importance_plots.png`: Gráficos de importância de features para cada variável-alvo.
    -   📄 `r2_performance_severidade.png`: Gráfico de barras comparando o R² dos modelos para predição de severidade.
    -   📄 `shap_summary_plots.png`: Gráficos de importância e distribuição de impacto do SHAP.
    -   📄 `pdp_fungus_plot.png`: Gráfico de Dependência Parcial mostrando o efeito médio de cada espécie de fungo.
-   **`/results/`**: Armazena as métricas de desempenho dos modelos em formato CSV.
    -   📄 `metricas_performance_severidade.csv`: Métricas (R², MAE, RMSE) para os modelos de predição de severidade.
    -   📄 `metricas_performance_comprimento.csv`: Métricas para os modelos de predição do comprimento da lesão.
    -   📄 `metricas_performance_largura.csv`: Métricas para os modelos de predição da largura da lesão.
-   **`/article/`**: Contém os arquivos-fonte do manuscrito.
    -   📄 `manuscrito.tex`: Código-fonte LaTeX do artigo científico.
    -   📄 `referencias_pt.bib`: Arquivo de bibliografia BibTeX.

## 📝 Observações Metodológicas

-   Todos os dados são **sintéticos**, gerados com base nos parâmetros estatísticos (médias e desvios-padrão) reportados no estudo de referência de **Silva (2023), *Espécies de Colletotrichum e Fusarium associadas a sintomas da podridão vermelha da cana-de-açúcar***.
-   A lógica de geração dos dados buscou refletir as interações biológicas plausíveis (e.g., diferentes níveis de agressividade patogênica, efeitos de coinfecção), mas é, por natureza, uma simulação controlada.
-   As dependências Python necessárias para executar os notebooks estão listadas no arquivo `requirements.txt`.

## 🚀 Como Utilizar

1.  **Clone o repositório:**
    ```bash
    git clone https://github.com/zolpy/scientific_article_0022.git
    cd scientific_article_0022
    ```
2.  **Instale as dependências:**
    ```bash
    pip install -r requirements.txt
    ```
3.  **Execute os notebooks:** Abra os notebooks na pasta `/notebooks/` utilizando Jupyter Lab ou Google Colab para replicar as análises.

## 📄 Como Citar

Se você utilizar este repositório, a base de dados ou os conceitos apresentados no artigo, por favor cite o trabalho original (a citação completa será atualizada após a publicação):

> Autor(es). (Ano). Análise Preditiva da Severidade da Podridão Vermelha em Cana-de-Açúcar Utilizando Dados Sintéticos e Modelos de Regressão Interpretáveis. *Nome do Periódico*, Volume(Edição), Páginas. DOI (se disponível)

## ⚖️ Licença

Este projeto está licenciado sob a [Licença MIT](LICENSE.md).

</details>

<details>
<summary>🇺🇸 English</summary>

# Scientific Article – Predictive Analysis of Sugarcane Disease Severity

This repository contains the synthetic dataset and source code (Jupyter notebooks) used in the analyses presented in the scientific article: **"Predictive Analysis of Red Rot Severity in Sugarcane Using Synthetic Data and Interpretable Regression Models"**.

The goal of this project is to demonstrate the feasibility of applying Machine Learning techniques to predict the severity of disease symptoms in sugarcane, using a robust, synthetic database grounded in a reference study on the pathogenicity of fungi from the *Colletotrichum* and *Fusarium* genera.

## 🎯 Repository Objective

This repository aims to ensure **full reproducibility** of the experiments and analyses described in the associated scientific article. It allows for the exploration, validation, or adaptation of predictive models for stalk rot severity and leaf lesion dimensions. It serves as a resource for researchers interested in applying machine learning to plant pathology and precision agriculture, particularly using synthetic datasets.

## 📁 Repository Structure

-   **`/data/`**: Contains the synthetic dataset.
    -   📄 `sugarcane_synthetic_data.xlsx`: Dataset with 10,000 records, simulating inoculation trials of different fungal species on sugarcane, with respective input variables (inoculation type, variety) and output variables (severity, lesion length, and width).
-   **`/notebooks/`**: Contains the Jupyter notebooks with the entire analysis workflow.
    -   📄 `01_synthetic_data_generation.ipynb`: Code for generating the synthetic dataset based on statistical parameters from the reference study.
    -   📄 `02_exploratory_analysis_and_feature_selection.ipynb`: Exploratory data analysis (Box Plots, Correlation Matrices) and feature selection based on Random Forest feature importance.
    -   📄 `03_regression_model_benchmarking.ipynb`: Training and evaluation of over 20 regression models to predict disease severity and leaf symptoms using cross-validation.
    -   📄 `04_model_interpretability_with_xai.ipynb`: Interpretable AI (XAI) analysis of the best predictive model for severity using SHAP and Partial Dependence Plot (PDP) analysis.
    -   📄 `05_prediction_on_new_scenarios.ipynb`: Final code that uses the best-trained models to make predictions on a set of new hypothetical scenarios.
-   **`/figures/`**: Contains visualizations generated by the notebooks.
    -   📄 `boxplot_severity_by_species.png`: Box plot of disease severity distribution by fungal species.
    -   📄 `feature_importance_plots.png`: Feature importance plots for each target variable.
    -   📄 `r2_performance_severity.png`: Bar chart comparing the R² scores of models for severity prediction.
    -   📄 `shap_summary_plots.png`: SHAP feature importance and impact distribution plots.
    -   📄 `pdp_fungus_plot.png`: Partial Dependence Plot showing the average effect of each fungal species.
-   **`/results/`**: Stores model performance metrics in CSV format.
    -   📄 `performance_metrics_severity.csv`: Metrics (R², MAE, RMSE) for severity prediction models.
    -   📄 `performance_metrics_length.csv`: Metrics for lesion length prediction models.
    -   📄 `performance_metrics_width.csv`: Metrics for lesion width prediction models.
-   **`/article/`**: Contains the source files for the manuscript.
    -   📄 `manuscript.tex`: LaTeX source code for the scientific article.
    -   📄 `references_en.bib`: BibTeX bibliography file.

## 📝 Methodological Notes

-   All data are **synthetic**, generated based on the statistical parameters (means and standard deviations) reported in the reference study by **Silva (2023), *Species of Colletotrichum and Fusarium associated with red rot symptoms in sugarcane***.
-   The data generation logic aimed to reflect plausible biological interactions (e.g., different levels of pathogenic aggressiveness, co-infection effects) but is, by nature, a controlled simulation.
-   The Python dependencies required to run the notebooks are listed in the `requirements.txt` file.

## 🚀 How to Use

1.  **Clone the repository:**
    ```bash
    git clone https://github.com/zolpy/scientific_article_0022.git
    cd scientific_article_0022
    ```
2.  **Install dependencies:**
    ```bash
    pip install -r requirements.txt
    ```
3.  **Run the notebooks:** Open the notebooks in the `/notebooks/` folder using Jupyter Lab or Google Colab to replicate the analyses.

## 📄 How to Cite

If you use this repository, the dataset, or the concepts presented in the article, please cite the original work (full citation will be updated upon publication):

> Author(s). (Year). Predictive Analysis of Red Rot Severity in Sugarcane Using Synthetic Data and Interpretable Regression Models. *Journal Name*, Volume(Issue), Pages. DOI (if available)

## ⚖️ License

This project is licensed under the [MIT License](LICENSE.md).

</details>
