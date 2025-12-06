Sistema de Alocação de IGHT 2025: Otimização de Demanda e Equidade Algorítmica
Este repositório contém o código-fonte, as análises e os artefatos desenvolvidos para o Trabalho Final da disciplina de Machine Learning do Centro Universitário Católica de Quixadá (Unicatólica).
  Sobre o Projeto
O projeto aborda o desafio logístico de distribuir Imunoglobulina Humana Antitetânica (IGHT), um insumo de alto custo e demanda intermitente, na rede pública de saúde (SUS). Diferente de vacinas comuns, a demanda por IGHT é estocástica (causada por acidentes).
Para resolver isso, desenvolvemos uma arquitetura híbrida que combina:
Método de Croston: Para previsão estatística de séries temporais com muitos zeros (demanda intermitente).
K-Means Clustering: Algoritmo de aprendizado não supervisionado para segmentar municípios em grupos logísticos (Críticos, Metropolitanos, Cauda Longa).
Índice de Vulnerabilidade e Risco (IVR): Um mecanismo de equidade algorítmica que utiliza pesos demográficos (Raça/Cor) para priorizar estoques em regiões com populações historicamente vulneráveis.
  Arquivos do Repositório
ModeloFInal.ipynb: O core do projeto. Um Jupyter Notebook contendo todo o pipeline de dados:
ETL: Leitura otimizada de grandes volumes de dados do DataSUS usando chunking.
Modelagem: Implementação manual e vetorial do Método de Croston e aplicação do K-Means via scikit-learn.
Visualização: Geração de gráficos de sazonalidade, distribuição de clusters e mapas de calor.
Relatório: Geração automática do plano de alocação por UF.
filtered_anti_tetano_chunked.csv: (Amostra de Dados) Arquivo contendo os dados pré-processados e filtrados, focados exclusivamente nos registros de "Imunoglobulina humana antitétano". Este arquivo é o resultado da etapa de limpeza e serve de entrada para o modelo.
👥 Autores

Ronald Klaive Borges da Silva 2023010035
José Tailan Silva Barbosa 2023010266
Jeferson Iure Samuel de Matos 2016010109
Derick de Oliveira Paiva 2023010543
Francisco Nogueira de Lima Junior 2023010460
Felipe Mesquita Pinto 2023010541


Tecnologias Utilizadas
Python 3.x
Pandas (Manipulação de Big Data)
Scikit-learn (K-Means e Pré-processamento)
Matplotlib & Seaborn (Visualização de Dados)
NumPy (Cálculo Numérico)
