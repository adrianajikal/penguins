# Projeto: Agrupamento Hierárquico - Penguins Dataset

## Descrição
Este é um projeto de Análise e Agrupamento de pinguins utilizando o dataset "penguins" da biblioteca Seaborn. O objetivo foi aplicar técnicas de **Clustering Hierárquico** para identificar padrões e separações naturais entre as espécies de pinguins.

## Dataset
- Fonte: Seaborn (sns.load_dataset('penguins'))
- Colunas principais:
    - species (espécie)
    - island (ilha)
    - bill_length_mm (comprimento do bico)
    - bill_depth_mm (profundidade do bico)
    - flipper_length_mm (comprimento da nadadeira)
    - body_mass_g (massa corporal)
    - sex (sexo)

## Objetivo
Realizar agrupamento hierárquico para identificar como as espécies e suas características morfológicas influenciam na formação de grupos naturais.

## Etapas
### 1. Exploração dos Dados
- Análise inicial das variáveis quantitativas e qualitativas.
- Tratamento de valores ausentes.

### 2. Normalização
- Normalização das variáveis quantitativas para ajustar escalas.

### 3. Agrupamento Hierárquico
- Teste inicial com **3 grupos**.
- Avaliação da distribuição das espécies em cada grupo.
- Interpretação e descrição dos grupos.

### 4. Reagrupamento com 5 grupos
- Realização de novo clustering com 5 grupos.
- Análise da composição de espécies e sexos em cada grupo.
- Análise crítica: O algoritmo capturou padrões naturais?

## Resultados
### Composição por Espécie e Sexo nos 5 Grupos
| Grupo | Espécie | Female | Male |
|---|---|---|---|
| 0 | Chinstrap | 20 | 34 |
| 1 | Gentoo | 9 | 61 |
| 2 | Adelie | 4 | 55 |
| 2 | Chinstrap | 9 | 0 |
| 3 | Gentoo | 49 | 0 |
| 4 | Adelie | 69 | 18 |
| 4 | Chinstrap | 5 | 0 |

### Interpretação
#### Grupo 0
- Exclusivamente **Chinstrap**.
- Bem balanceado entre machos e fêmeas.

#### Grupo 1
- Majoritariamente **Gentoo machos**.

#### Grupo 2
- Predominância de **Adelie machos** com algumas **Chinstrap fêmeas**.

#### Grupo 3
- Exclusivamente **Gentoo fêmeas**.

#### Grupo 4
- Principalmente **Adelie fêmeas**, com algumas **Chinstrap fêmeas** e poucos Adelie machos.

## Conclusão
- O agrupamento hierárquico capturou padrões biológicos reais:
    - **Separar espécies diferentes**.
    - **Separar machos e fêmeas em algumas espécies (Gentoo)**.
- As diferenças morfológicas (tamanho do corpo, comprimento do bico e da nadadeira) são fatores relevantes para a formação dos grupos.
- O algoritmo demonstrou capacidade de representar relações naturais entre as espécies, sexo e suas características físicas.

## Ferramentas Utilizadas
- Python 3.9+
- Pandas
- Seaborn
- Scipy (para clustering hierárquico)
- Matplotlib

## Como Executar
1. Clonar o repositório.
2. Executar o arquivo `penguins_clusters.ipynb`.
3. Explorar as visualizações e análises geradas.

## Autor
Projeto desenvolvido por Adriana Jikal, como parte do curso de Data Science da EBAC.

## Licença
Este projeto é livre para uso educacional.
