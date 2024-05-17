# Classificação de espécies de pinguins

![Imagem dos pinguins.](docs/assets/images/penguins.png)

O objetivo principal do projeto é realizar uma **análise comparativa de diferentes modelos de aprendizado de máquina** utilizando o conjunto de dados público "`Palmer Archipelago (Antarctica) penguin data`." Além disso, uma análise **exploratória de dados (EDA)** foi realizada para entender melhor as características dos pinguins. As variáveis do conjunto de dados incluem tanto qualitativas nominais (`species`, `island`, `sex`) quanto quantitativas contínuas (`bill_length_mm`, `bill_depth_mm`, `flipper_length_mm`, `body_mass_g`). As etapas de pré-processamento envolveram codificação de variáveis categóricas e tratamento de valores ausentes e outliers, além de normalização. A EDA revelou insights como a predominância da espécie Adelie, a maioria dos pinguins originários da ilha Biscoe, e a alta variabilidade no comprimento do bico, além de correlações interessantes entre as características físicas e as espécies de pinguins.

Foram utilizados quatro modelos de classificação (K-Nearest Neighbors, Support Vector Machine, Decision Tree e Random Forest) e suas performances foram avaliadas usando métricas como acurácia, precisão, recall e F1-score. A busca em grade pelos hiperparâmetros indicou que o modelo KNN apresentou o melhor desempenho. As ferramentas e bibliotecas utilizadas no projeto incluem Python, pandas, scikit-learn, seaborn, matplotlib e numpy. O próximo passo é criar um serviço para disponibilização do modelo, consolidando assim a aplicação prática dos resultados obtidos.


## Desenvolvedores
 - Madson Dias ([@omadson](http://github.com/omadson))


## Organização de diretórios


```
.
├── data/              # Diretório contendo todos os arquivos de dados
│   ├── external/      # Arquivos de dados de fontes externas
│   ├── interim/       # Arquivos de dados intermediários
│   ├── processed/     # Arquivos de dados processados
│   └── raw/           # Arquivos de dados originais, imutáveis
├── docs/              # Documentação gerada através da biblioteca mkdocs
├── models/            # Modelos treinados e serializados, predições ou resumos de modelos
├── notebooks/         # Diretório contendo todos os notebooks utilizados nos passos
├── references/        # Dicionários de dados, manuais e todo o material exploratório
├── src/               # Código fonte utilizado nesse projeto
│   ├── data/          # Classes e funções utilizadas para download e processamento de dados
│   ├── deployment/    # Classes e funções utilizadas para implantação do modelo
│   └── model/         # Classes e funções utilizadas para modelagem
├── app.py             # Arquivo com o código da aplicação do streamlit
├── pyproject.toml     # Arquivo de dependências para reprodução do projeto
├── poetry.lock        # Arquivo com sub-dependências do projeto principal
└── README.md          # Informações gerais do projeto

```
