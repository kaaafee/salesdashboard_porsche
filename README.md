# 🏎️ Porsche Sales Intelligence Dashboard

Um **Dashboard Executivo Interativo de Inteligência de Vendas** construído em HTML5, CSS3 puro e JavaScript com renderização gráfica dinâmica via **Chart.js (Canvas)**. O projeto analisa o desempenho comercial, depreciação, distribuição geográfica e ciclo operacional de veículos Porsche.

---

## 🎨 UI/UX & Design System

A interface foi concebida com base na identidade visual minimalista e de alta performance do **site oficial da Porsche**:

* **Theme:** *Dark Luxury* (fundo escuro de alto contraste para destacar os dados).
* **Palette:** *Porsche Black* (`#0A0A0A`), *Porsche Crimson Red* (`#D5001C`) como cor de destaque e acentos em dourado metálico.
* **Layout:** Design responsivo, estruturado com **CSS Grid** e **Flexbox**, cards de KPI com indicação tátil e navegação por abas sem recarregamento de página.

---

## 📊 Arquitetura e Páginas do Dashboard

O dashboard é dividido em **4 páginas/visões analíticas**:

### 1. Visão Geral (Overview)

* **KPIs Globais:** Volume Total de Vendas, Receita Bruta, Ticket Médio, Quilometragem Média e Taxa de Conclusão de Pedidos.
* **Evolução Temporal:** Gráfico combinado de barras e linhas (Receita em USD vs. Unidades Vendidas).
* **Performance de Produto:** Ranking *Top Models* mais vendidos.
* **Geografia Inicial:** Distribuição percentual de vendas por Estado (UF).

### 2. Análise por Produto

* **Curva de Depreciação:** Scatter Plot relacionando *Preço de Venda ($)* vs. *Quilometragem (mi)* para análise do impacto do uso no valor de revenda.
* **Valorização por Ano (MY):** Gráfico de linha demonstrando a evolução do preço médio por ano do modelo.
* **Mix de Vendas:** Segmentação de unidades por faixas de preço.

### 3. Análise Geográfica

* **Receita Regional:** Desempenho comparativo por regiões geograficamente agrupadas (Northeast, West, South, Midwest).
* **Tabela Dinâmica Auditável:** Visão hierárquica detalhada (*Estado $\times$ Cidade $\times$ Qtd Vendas $\times$ Receita Total $\times$ Ticket Médio*).

### 4. Status & Operacional

* **Funil de Pedidos:** Gráfico Polar/Donut rastreando o ciclo de vida da venda (*Delivered, In Transit, Pending, Cancelled, Shipped, etc.*).
* **Finanças & Pagamento:** Análise do mix de meios de pagamento (*Wire Transfer, Financing, Cash, Credit Card*).

---

## 🎛️ Recursos Interativos

* **Filtros Dinâmicos em Tempo Real:**
* Intervalo de Datas de Venda.
* Modelo do Veículo e Ano do Modelo (MY).
* **Hierarquia Geográfica Dinâmica:** A seleção do Estado (UF) filtra automaticamente a lista de Cidades disponíveis.
* Status da Entrega.
* Range Sliders para **Preço Máximo** e **Quilometragem Máxima**.


* **Motor de Dados In-Memory:** Todos os gráficos e KPIs reagem instantaneamente a qualquer combinação de filtros aplicados.

---

## 🛠️ Tecnologias Utilizadas

* **HTML5 Semantic Structure**
* **CSS3 Custom Properties (CSS Variables)**
* **JavaScript (ES6+)** — Manipulação DOM, filtragem de dados em memória e agregação estatística.
* **Chart.js** — Renderização de gráficos em elementos `<canvas>`.

