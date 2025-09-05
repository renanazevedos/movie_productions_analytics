
# Movie Productions Analytics

Projeto de Data Science para análise e modelagem preditiva de dados da indústria cinematográfica, com foco em apoiar decisões estratégicas de estúdios de cinema.

## Visão Geral

Este repositório reúne um pipeline completo de análise exploratória de dados (EDA), engenharia de variáveis e modelagem preditiva, utilizando técnicas de ciência de dados. O objetivo é identificar padrões relevantes, responder perguntas de negócio e recomendar estratégias para maximizar o sucesso de lançamentos cinematográficos.

## Estrutura do Projeto

- `data/raw/desafio_indicium_imdb.csv`: Base de dados original, contendo informações detalhadas sobre filmes (título, ano, classificação, duração, gênero, nota IMDb, sinopse, meta score, diretor, elenco, votos e faturamento).
- `modelo/modelo_nota_imdb_xgb_v1.pkl`: Modelo preditivo treinado (XGBoost) para estimativa da nota IMDb, pronto para uso em produção.
- `notebooks/eda.ipynb`: Notebook principal de EDA e modelagem, com roteiro analítico, visualizações avançadas, engenharia de variáveis e validação de modelos.
- `reports/eda.html`: Relatório interativo gerado a partir do notebook, facilitando a comunicação dos resultados.
- `environment.yml` / `requirements.txt`: Arquivos de dependências para ambiente Conda ou pip.

## Destaques do EDA (`notebooks/eda.ipynb`)

O notebook apresenta um roteiro analítico completo, incluindo:

- **Configuração Ambiente:** Importação de bibliotecas (Pandas, Seaborn, XGBoost, Scikit-learn, WordCloud, etc.) e definição de funções para análise estatística e visualização.
- **Inspeção e Limpeza dos Dados:** Análise de tipos, valores faltantes, estatísticas descritivas, identificação de outliers e tratamento de inconsistências.
- **Visualizações:** Geração de gráficos customizados (histogramas, boxplots, scatterplots, matriz de correlação, nuvem de palavras para sinopses) para explorar relações entre variáveis e padrões de sucesso.
- **Engenharia de Variáveis:** Criação e transformação de variáveis relevantes para modelagem, incluindo extração de informações textuais da sinopse e categorização de gêneros.
- **Modelagem Preditiva:** Desenvolvimento e avaliação de modelos (XGBoost, Random Forest), validação cruzada, análise de métricas (MAE, R²) e seleção do melhor modelo para estimativa da nota IMDb.
- **Reprodutibilidade e Documentação:** Funções auxiliares, comentários detalhados e salvamento do modelo final em formato `.pkl`.

## Como Executar

1. Clone o repositório:
	```powershell
	git clone <URL_DO_REPOSITORIO>
	```

2. Crie o ambiente Conda:
	```powershell
	conda env create -f environment.yml
	conda activate movie_productions_analytics
	```

	Ou instale as dependências via pip:
	```powershell
	pip install -r requirements.txt
	```

3. Execute o notebook `notebooks/eda.ipynb` para reproduzir a análise, visualizações e modelagem.

## Principais Ferramentas e Técnicas

- Python 3.x
- Jupyter Notebook
- Pandas, NumPy, Scikit-learn, XGBoost
- Matplotlib, Seaborn, WordCloud
- Engenharia de variáveis, validação cruzada, métricas de regressão

## Resultados e Insights

- Análise detalhada dos fatores que influenciam o sucesso de filmes.
- Identificação de padrões relevantes para recomendações estratégicas.
- Modelo preditivo para estimativa da nota IMDb.
- Relatórios visuais e documentação clara para stakeholders.

## Autor

Renan Azevedo 
Cientista de Dados
