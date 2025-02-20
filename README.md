# Descrição do Projeto

Desenvolver uma ferramenta que gere recomendações sobre regiões ideais para a prospecção de terrenos. Para essa ferramenta,
espera-se a identificação de oportunidades de negócios de forma ativa e com cenário competitivo favorável, ou seja, bairros 
com pouco estoque e condições ideais de demanda.

## Pasta "Instructions"
Contém os arquivos com as intruções do projeto
 - Prosta Nortis: contém a proposta da ita júnior(o que vamos fazer)
 - Termo de Programa - Modelo de Recomendação: contém o que a empresa pediu
 - RELATÓRIO MVP: contém um projeto passado que possui semelhanças com esse projeto para que possamos
ter um norte inicial (OS ARQUVIVOS .ZIP CONTÉM AS BRANCHES UTILIZADAS NO PROJETO "RELATÓRIO MVP"
)
 - https://github.com/denilsonsoares/IoT_Refeitorio/tree/main/plataforma: link de um projeto que possui estrutura
base para este.

![img.png](img.png) 
![img_1.png](img_1.png)

# Estrutura de Pastas
## 1. data/
- raw/: Armazena os dados brutos, ou seja, os dados coletados de fontes originais sem qualquer tratamento ou pré-processamento.
- processed/: Contém os dados que já passaram por algum tipo de processamento ou limpeza, prontos para serem utilizados na análise ou modelagem.
## 2. models/
- Armazena os modelos de machine learning treinados ou em desenvolvimento. Isso pode incluir arquivos de modelos serializados (por exemplo, modelos .pkl do scikit-learn) e scripts relacionados aos modelos.
## 3. notebooks/
- Contém notebooks Jupyter utilizados para exploração inicial dos dados, prototipagem de modelos e análises ad-hoc. Esses notebooks são úteis para documentação e experimentação.
## 4. src/
- init.py: Torna o diretório um pacote Python, permitindo a importação dos módulos.
- data_collection.py: Define a classe e funções responsáveis pela coleta de dados de diferentes fontes.
- data_processing.py: Contém a classe e funções para o processamento e limpeza dos dados.
- data_analysis.py: Inclui a classe e funções para análise exploratória dos dados e visualizações.
- machine_learning.py: Define a classe e funções para a criação, treinamento e avaliação de modelos de machine learning.
- utils.py: Contém funções utilitárias que são usadas em múltiplas partes do projeto, como carregamento de dados, salvamento de arquivos, etc.
## 5. streamlit_app/
- init.py: Torna o diretório um pacote Python.
- main.py: Arquivo principal que configura a aplicação Streamlit, definindo as diferentes abas e integrando as funcionalidades de coleta, processamento, análise e machine learning.
- pages/: Diretório que contém as páginas individuais do aplicativo Streamlit, cada uma responsável por uma parte específica do fluxo de trabalho:
- data_collection_page.py: Página de coleta de dados, utilizando a classe DataCollector do módulo data_collection.py.
- data_processing_page.py: Página de processamento de dados, utilizando a classe DataProcessor do módulo data_processing.py.
- data_analysis_page.py: Página de análise de dados, utilizando a classe DataAnalyzer do módulo data_analysis.py.
- machine_learning_page.py: Página de machine learning, utilizando a classe MachineLearningModel do módulo machine_learning.py.
## 6. .gitignore
- Arquivo de configuração do Git que especifica quais arquivos ou diretórios devem ser ignorados pelo controle de versão, como dados brutos, modelos treinados, arquivos temporários, etc.
## 7. README.md
- Arquivo de documentação do projeto, fornecendo uma visão geral do projeto, instruções de instalação, uso, estrutura do projeto e outras informações relevantes.
## 8. requirements.txt
- Lista de dependências do projeto que precisam ser instaladas para executar o código, como bibliotecas Python (por exemplo, Streamlit, pandas, scikit-learn).

## Resumo das Funções
- data/: Armazenamento de dados brutos e processados.
- models/: Armazenamento de modelos de machine learning.
- notebooks/: Prototipagem e exploração de dados.
- src/: Implementação das classes e funções principais do projeto.
- streamlit_app/: Implementação da aplicação Streamlit com diferentes abas para cada parte do fluxo de trabalho.
- .gitignore: Configuração de exclusões para o controle de versão.
- README.md: Documentação do projeto.
- requirements.txt: Dependências do projeto.

### Requiments.txt
- pip install -r requirements.txt

## Nomenclatura dos Arquivos e Pastas

Utilize nomes descritivos e em inglês para arquivos e pastas.
Siga convenções de nomenclatura como snake_case para arquivos e camelCase para classes.

## Rodar o projeto
- cd streamlit_app
- streamlit run main.py