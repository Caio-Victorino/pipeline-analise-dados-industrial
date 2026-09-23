# 🏭 Pipeline de Análise de Dados e Engenharia Industrial com Python

## 📌 Visão Geral do Projeto
Este projeto consiste no desenvolvimento de um pipeline ETL (Extract, Transform, Load) automatizado para processamento e análise de dados do chão de fábrica. 

O sistema consolida registros de produção de múltiplas linhas de montagem, cruza dados cadastrais de equipamentos, trata telemetria temporal, calcula indicadores operacionais (KPIs de qualidade e downtime) e gera relatórios executivos automatizados em formato Excel multi-abas.

---

## 🛠️ Tecnologias Utilizadas
- **Linguagem:** Python
- **Manipulação de Dados:** Pandas, NumPy
- **Manipulação Temporal:** datetime, Timedelta
- **Automação de Saída:** openpyxl, pd.ExcelWriter
- **Ambiente:** Google Colab

---

## ⚙️ Funcionalidades do Pipeline
1. **Consolidação de Dados:** Empilhamento (`pd.concat`) e cruzamento relacional (`pd.merge`) de bases de produção e cadastro de setores.
2. **Séries Temporais:** Conversão de datas (`pd.to_datetime`), cálculo de tempo de ciclo em minutos e suporte a Média Móvel (`.rolling()`) e Reamostragem (`.resample()`).
3. **KPIs Industriais:** Cálculo de volume total produzido, Taxa de Refugo (%) e classificação condicional de lotes (`np.where()`).
4. **Relatório Executivo:** Exportação automatizada em Excel (`.xlsx`) com abas segmentadas (`Base_Consolidada` e `Lotes_Reprovados`).

---

## 📊 Principais Resultados
- **Setor Crítico Detectado:** Funilaria.
- **Lotes Reprovados (Refugo > 5%):** Lote 5002 (7,27%) e Lote 5005 (10,00%).

---

## ✒️ Autor
Desenvolvido por **Caio Victorino** — Estudante de Engenharia de Inteligência Artificial.
