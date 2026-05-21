# # ANÁLISE DO MERCADO DE TECNOLOGIA IOT NO BRASIL
Sistema de recomendação para qualificação de potenciais clientes em tecnologia IoT no Brasil

## Apresentação
Link do Youtube com apresentação Final
[Youtube](https://youtu.be/U5QHtly2-5Y)

## Descrição do Projeto
Este trabalho apresenta o desenvolvimento de um sistema de recomendação voltado para a prospecção de empresas no cenário B2B brasileiro, utilizando a base de dados pública de CNPJs do Ministério da Fazenda. O objetivo é transformar a busca por novos clientes em um processo orientado a dados (data-driven), superando as limitações dos métodos tradicionais de marketing. A metodologia proposta consiste no processamento de Big Data para identificar organizações similares a uma empresa-alvo escolhida pelo usuário, permitindo filtros por localização e porte. O estudo destaca-se pela abordagem técnica comparativa, analisando o desempenho e a precisão dos algoritmos K-Nearest Neighbors (KNN) e Cosine Similarity através de uma prova de conceito. Os resultados esperados incluem a otimização da geração de leads e a validação de modelos de similaridade aplicados a dados cadastrais públicos.

## OBJETIVO GERAL
Desenvolver um sistema de recomendação de empresas B2B fundamentado em análise de similaridade para que se identifiquem organizações com perfis operacionais e estruturais análogos a uma empresa de referência.

## Estrutura do Repositório

A organização dos arquivos no repositório segue a seguinte estrutura:

```
├── config/                                               # Descritivo das Configurações utilizadas aos softwares utilizados no projeto, caso houver
├── dataset/                                              # Notebooks Jupyter com análises pertinentes ao projeto
├── ├── about.txt                                         # Instruções sobre como acessar ao repositório dos dados utilizados
├── processamento/                                        # Local para armazenar os códigos utilizados em cada etapa do projeto
├── ├── about.txt                                         # Instruções sobre o repositório de processamento
├── ├── NoteBook_Ricardo.ipynb                            # Notebooks contendo código python aplicando dicionário de termos no dataset
├── reports/                                              # Local para armazenar os modelos de Relatórios (Estático e Dinâmico) e apresentações
├── ├── about.txt                                         # Instruções sobre o repositório de relatórios
├── ├── ProjetoAplicadoIII__ArtigoAcademico_A4__V1_0.pdf  # Documento academico com a entrega final
├── LICENSE                                               # Licença do projeto
├── README.md                                             # Arquivo explicativo do projeto (este documento)

```

## Objetivos
O estudo visa:
1. OBJETIVO GERAL - Desenvolver um sistema de recomendação de empresas B2B fundamentado em análise de similaridade para que se identifiquem organizações com perfis operacionais e estruturais análogos a uma empresa de referência.
2. OBJETIVO ESPECIFICO - Coletar e tratar dados estruturados e semiestruturados provenientes da base de "Dados Abertos" do Governo Federal para que se componha um ecossistema de informações confiável entre os anos de 2021 e 2026.
3. OBJETIVO ESPECIFICO - Implementar algoritmos de filtragem de informação, como K-Nearest Neighbors (KNN) e Cosine Similarity, para que se avalie qual métrica de distância melhor representa a similaridade em dados cadastrais empresariais
4. OBJETIVO ESPECIFICO - Desenvolver filtros parametrizáveis de abrangência geográfica e segmentação de porte para que o usuário restrinja o escopo das recomendações conforme sua necessidade estratégica de mercado
5. OBJETIVO ESPECIFICO - Validar a eficácia do sistema por meio de uma Prova de Conceito (PoC) para que se comprove a viabilidade técnica e a precisão da solução proposta
6. OBJETIVO ESPECIFICO - Estruturar um sistema de pontuação (scoring) com pesos variáveis para que se hierarquize a relevância dos leads gerados para o usuário final, consolidando uma solução de inteligência de mercado

## Datasets Utilizados

**Fontes de Dados**
* Refeita Federal
 [Empresas consultável por CNPJ](https://arquivos.receitafederal.gov.br/dados/cnpj/dados_abertos_cnpj/2026-01/)

**Metadados**
* Período de coleta: Dados mais recentes disponíveis até Janeiro de 2026.
* Limitações:
  * Alguns dados podem estar incompletos ou desatualizados.
  * Dados públicos sujeitos a limitações de granularidade.
* Organização:
  * Dados brutos estão na pasta data/raw/.
  * Dados tratados estão na pasta data/processed/.

## Tecnologias Utilizadas
O projeto faz uso das seguintes ferramentas:
  * pandas → manipulação de dados tabulares (DataFrame)
  * numpy → operações matemáticas e arrays
  * datetime → manipulação de datas
  * re → limpeza de texto (regex)
  * warnings → controle de avisos do Python
  * pyspark.sql.SparkSession → cria sessão Spark
  * pyspark.sql.functions (F) → funções SQL (filtros, colunas, etc.)
  * LabelEncoder → transforma categorias em números
  * StandardScaler → normaliza os dados
  * TfidfVectorizer → transforma texto em números (NLP)
  * NearestNeighbors → busca empresas similares (KNN)
  * KMeans → clustering (segmentação)
  * PCA → redução de dimensionalidade
  * cosine_similarity → mede similaridade entre empresas
  * matplotlib → gráficos básicos
  * seaborn → gráficos estatísticos mais bonitos
  * time → medir tempo de execução


Para instalar as dependências, execute:

```
pip install -r requirements.txt
```

## Como Reproduzir o Projeto
1. Clone este repositório:
```
git clone https://github.com/seu-repositorio/mack_ds_projeto_aplicado_iii.git
```
2. Navegue até a pasta do projeto:
```
cd mack_ds_projeto_aplicado_iii
```
Instale as dependências listadas no arquivo requirements.txt:
```
pip install -r requirements.txt
```
Execute os notebooks na pasta notebooks/ para reproduzir as análises.

## Cronograma do Projeto
| Atividade |	Data de Conclusão |
|-----------|-------------------|
| Artigo Acadêmico | W21/2026 |
| Estabelecimento do repositório | W9/2026 |
| Coleta de dados | W9/2026 |
| Preparação dos dados | W14/2026 |
| Análise exploratória | W14/2026 |
| Implementação Algoritmos de recomendação | W16/2026 |
| Treinamento e Teste | W17/2026 |
| Apresentação em vídeo | W21/2026 |
| Relatório final | W21/2026 |

## Equipe
Este projeto foi desenvolvido como parte da disciplina "Projeto Aplicado III" do curso "Tecnologia em Banco de Dados: Análise, Mineração e Engenharia de Dados" da Universidade Presbiteriana Mackenzie.

**Integrantes:**
* Gustavo Azevedo Gomyde
* Ricardo de Oliveira Vieira Franco

**Docente Orientador:**
* Prof. Dr. Gustavo Scalabrini Sampaio

## Licença
Este projeto está licenciado sob a licença MIT. Consulte o arquivo `LICENSE` para mais detalhes.
