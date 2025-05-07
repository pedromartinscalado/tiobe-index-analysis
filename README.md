# TIOBE Index Analysis

Este repositório apresenta uma análise completa do TIOBE Programming Community Index (Março 2025), incluindo coleta, processamento, visualização e relatórios. Os principais objetivos são:

- Demonstrar diferentes técnicas de visualização em Python (Matplotlib, Seaborn, Plotly, Cufflinks).
- Comparar a popularidade das 10 principais linguagens entre março de 2024 e março de 2025.
- Fornecer código reprodutível e documentação clara para usuários e colaboradores.

## Estrutura de Pastas
tiobe-ratings/
│   ├── tioberatings.ipynb     # Notebook principal de análise
├── README.md                 # Documentação deste repositório
└── requirements.txt          # Dependências do projeto


## Como Reproduzir
1. Clone este repositório:
   ```bash
   git clone https://github.com/pedromartinscalado/tiobe-index-analysis.git
   cd tiobe-index-analysis
   
2. Crie e ative um ambiente virtual:
   ```bash
   python -m venv venv
   source venv/bin/activate  # Windows: venv\Scripts\activate

3. Instale as dependências:
   ```bash
   pip install -r requirements.txt

4. Execute os notebooks ou scripts:
   ```bash
    jupyter nbconvert notebooks/tioberatings.ipynb --to html --output reports/tiobe_analysis.html
    jupyter nbconvert notebooks/tioberatings.ipynb --to pdf --TemplateExporter.exclude_input=True --output     
    reports/tiobe_analysis.pdf

5. Principais Visualizações
1 - Gráfico de Barras: ranking top 10 linguagens (Março 2025) com Matplotlib e Seaborn, incluindo anotações de percentuais.

2 - Gráfico Interativo (Plotly): barras horizontais interativas, com tooltips e valores externos.

3 - Comparação Temporal: barras agrupadas comparando ratings de março de 2024 vs março de 2025.

4 - Pie Chart: distribuição percentual das 10 principais linguagens.

5 - Subplots: combinação de Seaborn e Plotly em múltiplas visualizações.

6 - Stem Plot: gráfico de caule para evidenciar variações de rating.

7 - Stack Plot: área empilhada comparando os dois períodos.

8 - Scatter Plot: dispersão ratings 2024 vs 2025 com linha de referência y=x.

9 - Cufflinks: barras comparativas usando Plotly Graph Objects.

10 - Heatmap: correlação e comparação de ratings entre os dois anos.

6. Dependências Principais
pandas
matplotlib
seaborn
plotly
cufflinks

```bash
Nota: pip freeze > requirements.txt
