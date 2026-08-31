# Análise Prática de Datasets do Setor de Energia
 **Soluções em Energias Renováveis e Sustentáveis**  
- Aplicação prática de preparação de dados com **Orange Data Mining** e análise exploratória com **Python & Pandas**.



## Atividade
Esta atividade busca aplicar os procedimentos trabalhados em aula para preparar, inspecionar e analisar diferentes conjuntos de dados do setor de energia, relacionando cada operação realizada ao contexto do dataset.

Os dados foram inicialmente processados no **Orange Data Mining** e exportados em arquivos `.csv`. Em seguida, foram analisados em ambiente Python via **Jupyter Notebook**, utilizando a biblioteca **Pandas**.

---

## Datasets Analisados e Fontes
**crianos a pasta amostras para armazenar os arquivos já filtrados pelo Orange**

 1. **Appliances Energy Prediction** | [UCI Machine Learning Repository](https://archive.ics.uci.edu/ml/datasets/Appliances+energy+prediction) | Consumo residencial de eletrodomésticos com variáveis ambientais de temperatura e umidade.
 2.  **Steel Industry Energy Consumption** | [UCI Machine Learning Repository](https://archive.ics.uci.edu/ml/datasets/Steel+Industry+Energy+Consumption+Dataset) | Consumo energético de uma indústria siderúrgica com variáveis de potência reativa, fator de potência e tipo de carga. |
 3.  **Power Consumption of Tetouan City** | [UCI Machine Learning Repository](https://archive.ics.uci.edu/ml/datasets/Power+Consumption+of+Tetouan+City) | Consumo elétrico em três zonas de distribuição da cidade de Tétouan, Marrocos, e dados meteorológicos. |
 4.   **Solar Power Generation Data** | [Kaggle](https://www.kaggle.com/datasets/anikannal/solar-power-generation-data) | Dados de geração (CC e CA) e rendimento diário de inversores de uma usina fotovoltaica. |
 5.    **Wind & Solar Energy Production Dataset** | [Kaggle](https://www.kaggle.com/datasets) | Produção temporal comparativa entre energia eólica e energia solar. |
 6.**Individual Household Electric Power Consumption** | [UCI Machine Learning Repository](https://archive.ics.uci.edu/ml/datasets/Individual+household+electric+power+consumption) | Medições de alta frequência de consumo residencial, tensão, corrente e submedições por circuito. |



## Estrutura do Notebook 
O notebook está dividido em células identificadas por títulos em Markdown para cada um dos 6 datasets abordados na aula, contendo:
1. Inspeção inicial com `.head()`, `.shape`, `.info()` e `.describe()`.
2. Renomeação de colunas para nomes padronizados em português.
3. Cálculo de métricas de referência (picos de consumo, médias).
4. Aplicação de filtros compostos/condicionais.
5. Contagem e percentual de registros filtrados.
6. **Interpretação e análise técnica** contextualizada dos resultados.

# Desafio Extra

## Visão Geral do Projeto
Este projeto realiza uma análise exploratória e descritiva do comportamento da demanda de carga elétrica na **Área SP (São Paulo)**, utilizando dados oficiais consumidos diretamente da API pública de Carga Verificada do **Operador Nacional do Sistema Elétrico (ONS)**.

O objetivo é mapear o padrão de consumo, identificar os momentos de alta demanda (picos) e fornecer insumos para o planejamento e operação do Sistema Interligado Nacional (SIN).



## Resumo Executivo dos Dados

* **Fonte de Dados:** API Pública do ONS (`apicarga.ons.org.br`)
* **Região Analisada:** SP — São Paulo
* **Período de Análise:** 01/08/2025 a 07/08/2025
* **Frequência das Medições:** A cada 30 minutos (336 registros totais)


