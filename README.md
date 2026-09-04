---

## ✨ Funcionalidades Chave

- 📊 **KPI Cards Executivos**: Indicadores dinâmicos no topo da planilha com atualização automática baseada em fórmulas (`SUM`, `AVERAGE`).
- 🍕 **Distribuição por Categoria**: Gráfico de pizza interativo acoplado à tabela de categorias (*Consoles*, *Games*, *Acessórios* e *Game Pass*).
- 📈 **Análise Temporal de Tendências**: Gráfico de linhas focado na evolução histórica mensal por segmento de mercado.
- 🌍 **Performance Regional & Share**: Gráfico de barras verticais para comparação entre metas e realizado por território (NA, EMEA, LATAM, APAC).
- 🎨 **Design System Executivo**:
  - Paleta baseada em **Xbox Green (`#107C41`)** e **Dark Slate Navy (`#0F172A`)**.
  - Formatação condicional e zebrada para facilitar a leitura.
  - Tipografia padronizada em *Segoe UI*.
  - Grade de exibição mantida e colunas dimensionadas automaticamente.

---

## 🗂 Arquitetura da Planilha (`.xlsx`)

O arquivo gerado é estruturado em **6 abas especializadas**:

| Aba | Descrição |
|---|---|
| `Dashboard Executivo` | Visão C-Level contendo KPIs, Tabelas Consolidadas e os Gráficos Principais (Pizza, Barras e Linha). |
| `Vendas Detalhadas` | Base granular de transações individuais com controle de SKU, Canal de Venda e Descontos. |
| `Serviços e Subscriptions` | Mapeamento de receitas recorrentes do Game Pass (Ultimate, PC, Core) e Cloud Gaming. |
| `Hardware & Periféricos` | Controle de estoque, custo de fabricação, preço final e margem unitária por dispositivo. |
| `Desempenho Regional` | Acompanhamento de metas de vendas por gerenciamento regional. |
| `Evolução Mensal` | Dados consolidados mês a mês para suporte ao gráfico de tendência temporal. |

---

## 🛠 Tecnologias e Ferramentas

- **Linguagem**: Python 3.10+
- **Manipulação de Planilhas**: `openpyxl`
- **Engenharia de Dados & Fórmulas**: Fórmulas nativas do Excel (`SUMIFS`, `AVERAGE`, `SUM`) garantindo leveza e dinamismo.
- **Visualização de Dados**: Módulos de gráficos `PieChart`, `BarChart` e `LineChart` via `openpyxl.chart`.

---

## 🚀 Como Executar o Gerador

### Pré-requisitos

Certifique-se de ter o Python instalado na sua máquina:

```bash
python --version
