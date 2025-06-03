# 🎬 Análise Comparativa de Plataformas de Streaming

## 🔍 Visão Geral

Este projeto mergulha no universo dos gigantes do streaming para desvendar padrões, tendências e insights sobre os catálogos da **Netflix**, **HBO Max**, **Amazon Prime Video** e **Apple TV+**. 

Através de uma análise meticulosa, exploramos como cada plataforma posiciona seu conteúdo, quais gêneros dominam seus catálogos e como as avaliações do IMDb revelam a qualidade percebida pelos usuários.

## 🎯 Objetivo

- **Comparar** estratégias de conteúdo entre as principais plataformas
- **Identificar** padrões de distribuição por gênero e tipo de conteúdo
- **Analisar** qualidade através das avaliações IMDb
- **Revelar** insights sobre o mercado de streaming atual

## 📊 Plataformas Analisadas

| Plataforma | Conteúdos Analisados | Destaque |
|------------|---------------------|----------|
| **Netflix** | 21.082 títulos | Maior diversidade de conteúdo |
| **Amazon Prime** | 71.280 títulos | Maior volume absoluto |
| **HBO Max** | 9.575 títulos | Foco em qualidade premium |
| **Apple TV+** | 18.131 títulos | Catálogo mais curado |

## 🗂️ Estrutura do Projeto

```
STREAMING/
├── 📁 analise_exploratoria/          # Notebooks de análise por plataforma
│   ├── 📓 analise_apple.ipynb        # Análise Apple TV+
│   ├── 📓 analise_hbo.ipynb          # Análise HBO Max  
│   ├── 📓 analise_netflix.ipynb      # Análise Netflix
│   └── 📓 analise_prime.ipynb        # Análise Prime Video
│
├── 📁 Dados/                         # Datasets originais
│   ├── 📄 data_apple_tv.csv
│   ├── 📄 data_hbo_max.csv
│   ├── 📄 data_netflix.csv
│   └── 📄 data_prime_video.csv
│
├── 📁 Dados_tratados/                # Datasets limpos
│   ├── 📄 data_hbo_clean.csv
│   ├── 📄 data_netflix_clean.csv
│   ├── 📄 data_prime_video_clean.csv
│   └── 📄 df_apple_clean.csv
│
├── 📁 Dados_tratados_ML/             # Dados preparados para ML
│   └── 📄 data_netflix_cleanML.csv
│
└── 📁 Visualizações/                 # Análises comparativas
    ├── 📓 diferencas_streamings.ipynb
    ├── 📓 ranking_platform.ipynb
    └── 📋 streaming_dicionario.md
```

## 🛠️ Metodologia

### 1. **Limpeza e Tratamento**
- Remoção de registros sem título
- Imputação inteligente de avaliações IMDb baseada em gênero e década
- Padronização de formatos e tipos de dados
- Tratamento de valores ausentes

### 2. **Análise Exploratória**
- Distribuição por tipo de conteúdo (filmes vs séries)
- Mapeamento de gêneros mais populares
- Análise temporal de lançamentos
- Avaliação de qualidade por plataforma

### 3. **Insights Comparativos**
- Ranking de plataformas por qualidade média
- Identificação de nichos e especializações
- Padrões de distribuição temporal

## 📈 Principais Descobertas

- **Drama** domina todas as plataformas (18-22% do conteúdo)
- **Prime Video** tem o maior volume, mas **HBO Max** as melhores avaliações
- **Apple TV+** mantém um catálogo mais enxuto e seletivo
- **Netflix** oferece a maior diversidade de gêneros

## 🔧 Tecnologias Utilizadas

- **Python 3.11**
- **Pandas** - Manipulação de dados
- **NumPy** - Computação numérica  
- **Re** - Expressões regulares
- **Collections.Counter** - Contagem otimizada
- **Jupyter Notebooks** - Análise interativa

## 🚀 Como Executar

1. Clone o repositório
```bash
git clone [seu-repositorio]
cd STREAMING
```

2. Instale as dependências
```bash
pip install pandas numpy
```

3. Execute os notebooks na ordem:
   - Primeiro: notebooks individuais em `analise_exploratoria/`
   - Depois: análises comparativas em `Visualizações/`

## 🎓 Contexto Acadêmico

Este projeto foi desenvolvido como **atividade de conclusão do módulo de Python para Análise de Dados** da **Digital College**, sob orientação da professora **Nayara Valevskii**. 

O desafio proposto foi aplicar conceitos fundamentais de manipulação de dados, limpeza e análise exploratória em um dataset real e relevante do mercado de entretenimento.

## 🚀 Próximos Passos: Machine Learning

### **Aplicação Streamlit em Desenvolvimento**

O futuro deste projeto contempla a criação de uma **aplicação web interativa** usando Streamlit, que transformará esta análise em uma ferramenta prática para usuários finais.

#### **Funcionalidades Planejadas:**
- 🎯 **Sistema de Recomendação Inteligente**
  - Input: Gênero preferido pelo usuário
  - Output: Lista personalizada de filmes/séries rankeados

- ⭐ **Ranking por Qualidade IMDb**
  - Filtragem automática pelos títulos mais bem avaliados
  - Visualização de scores e número de votos

- 🔍 **Interface Intuitiva**
  - Filtros por plataforma, ano, tipo de conteúdo
  - Comparação lado a lado entre streamings
  - Métricas de qualidade em tempo real

#### **Tecnologias Futuras:**
- **Streamlit** - Interface web responsiva
- **Scikit-learn** - Algoritmos de recomendação
- **Pandas/NumPy** - Backend de dados
- **Plotly** - Visualizações interativas

## 💡 Visão de Futuro

Este projeto evolui de uma análise exploratória para uma **solução prática de recomendação**, combinando insights de dados com experiência do usuário. 

A meta é criar um assistente inteligente que não apenas mostra "o que assistir", mas "**onde** assistir o **melhor** conteúdo disponível".

---

*"Dos dados à decisão: transformando análise em experiência personalizada para cada usuário."*
