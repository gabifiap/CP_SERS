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
 6.    **Individual Household Electric Power Consumption** | [UCI Machine Learning Repository](https://archive.ics.uci.edu/ml/datasets/Individual+household+electric+power+consumption) | Medições de alta frequência de consumo residencial, tensão, corrente e submedições por circuito. | obs: A mostra 6 não foi possivel carregar aqui no github como csv, por conta do tamanho...



## Estrutura do Notebook 
O notebook está dividido em células identificadas por títulos em Markdown para cada um dos 6 datasets abordados na aula, contendo:
1. Inspeção inicial com `.head()`, `.shape`, `.info()` e `.describe()`.
2. Renomeação de colunas para nomes padronizados em português.
3. Cálculo de métricas de referência (picos de consumo, médias).
4. Aplicação de filtros compostos/condicionais.
5. Contagem e percentual de registros filtrados.
6. **Interpretação e análise técnica** contextualizada dos resultados.

# Desafio Extra
Este relatório apresenta a análise exploratória e descritiva do comportamento da carga de energia elétrica na Área SP (São Paulo), cobrindo o período de 01/08/2025 a 07/08/2025. Os dados analisados foram consumidos diretamente da API pública de Carga Verificada do Operador Nacional do Sistema Elétrico (ONS).

## Visão Geral do Projeto
Objetivos Principais:
- *Mapeamento do Padrão Operacional*: Mapear os indicadores fundamentais (carga média, mínima, máxima e mediana) do sistema no período.
- *Caracterização de Picos de Demanda*: Identificar e quantificar os registros que superaram o limiar de alta demanda (20.866,78 MW), isolando o momento de maior solicitação da rede.
- *Avaliação por Critérios Comparativos*: Confrontar o regime de alta demanda com métricas secundárias de operação (registros acima da carga média global de 17.870,83 MW).
- *Suporte ao Planejamento*: Fornecer insumos descritivos para a gestão e planejamento de curto prazo do Sistema Interligado Nacional (SIN).

Diretriz Metodológica Rígida:
Seguindo os critérios de auditoria técnica do setor elétrico, o relatório fundamenta-se EXCLUSIVAMENTE nos dados observados no conjunto retornado. Variações operacionais e momentos de pico são tratados puramente sob a ótica descritiva; hipóteses externas (como variações climáticas, temperatura ou dinâmicas industriais) não são apresentadas como fatos, uma vez que não constam na base de dados de Carga Verificada fornecida.


## Resumo Executivo dos Dados

* **Fonte de Dados:** API Pública do ONS (`apicarga.ons.org.br`)
* **Região Analisada:** SP — São Paulo
* **Período de Análise:** 01/08/2025 a 07/08/2025
* **Frequência das Medições:** A cada 30 minutos (336 registros totais)


