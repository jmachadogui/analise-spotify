# Pré-processamento de Dados - Spotify Tracks Dataset

Projeto de pré-processamento de dados desenvolvido para a disciplina **Tópicos Avançados em Computação IV**.

**Participantes:**
- Adriano André da Silva
- Gustavo Henrique de Brum
- Guilherme Júnior Machado
- João Pedro Oliveira Barbosa
- Jorge Miguel Eberhard da Conceição

---

## Instalação de Dependências

Certifique-se de ter o Python instalado, então execute:

```bash
pip install -r requirements.txt
```

As bibliotecas utilizadas são:
- `pandas`
- `numpy`
- `matplotlib`
- `seaborn`
- `scikit-learn`

---

## Como Rodar

### Script Python

```bash
python script.py
```

### Notebook Jupyter (execução via terminal)

```bash
jupyter nbconvert --to notebook --execute "Tópicos_IV_Relatório_Pré_Processamento_Spotify.ipynb" --output "Tópicos_IV_Relatório_Pré_Processamento_Spotify.ipynb"
```

### Notebook Jupyter (interface interativa)

```bash
jupyter notebook "Tópicos_IV_Relatório_Pré_Processamento_Spotify.ipynb"
```

---

## Outputs

### Arquivos CSV

| Arquivo | Descrição |
|---|---|
| `spotify_clean.csv` | Dataset após limpeza e pré-processamento |
| `spotify_normalized.csv` | Dataset com variáveis numéricas normalizadas (Min-Max) |

### Gráficos (pasta `resultados/`)

| Arquivo | Descrição |
|---|---|
| `01_valores_ausentes.png` | Quantidade de valores ausentes por coluna |
| `02_distribuicoes.png` | Distribuição das variáveis numéricas com linha de média |
| `03_boxplots.png` | Boxplots das variáveis numéricas |
| `04_correlacao.png` | Matriz de correlação entre variáveis numéricas |
| `05_correlacao_popularity.png` | Correlação de cada variável com `popularity` |
| `06_top_generos.png` | Top 10 gêneros musicais mais frequentes |
| `07_energy_vs_popularity.png` | Dispersão entre `energy` e `popularity` |
| `08_danceability_vs_valence.png` | Dispersão entre `danceability` e `valence` |
| `09_popularidade_media_genero.png` | Popularidade média por gênero musical |
| `10_popularidade_media_explicit.png` | Popularidade média por conteúdo explícito |

---

## Etapas do Pré-processamento

1. **Leitura do dataset** — carregamento do `dataset.csv` e inspeção inicial
2. **Análise inicial** — tipos de variáveis, valores ausentes, duplicatas e estatísticas descritivas
3. **Pré-processamento** — remoção de duplicatas, tratamento de ausentes, conversão de duração, remoção de colunas irrelevantes, filtragem por popularidade, validação de intervalos, clipagem de outliers (IQR) e normalização Min-Max
4. **Análise estatística e correlação** — estatísticas descritivas dos dados tratados e geração de gráficos
