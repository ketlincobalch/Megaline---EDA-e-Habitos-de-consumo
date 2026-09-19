# Megaline---EDA-e-Habitos-de-consumo
Projeto de aplicação de testes estatísticos para identificar o plano pré-pago de maior rentabilidade, com resultado de 25,8% de diferença média de receita entre os planos Ultimate e Surf. Desenvolvido em Python com Pandas, NumPy e SciPy, incluindo limpeza de dados, visualização com histogramas e validação de hipóteses.

# Análise Estatística de Planos de Telecomunicações | Megaline

## Objetivo

Identificar qual dos planos pré-pagos da Megaline (Surf ou Ultimate) gera maior receita para apoiar decisões de investimento em marketing e publicidade.

## Contexto de Negócio

A Megaline oferece dois planos pré-pagos para seus clientes:

- Surf
- Ultimate

O departamento comercial precisava determinar qual plano apresentava melhor desempenho financeiro para direcionar investimentos publicitários e estratégias de aquisição de clientes.

A análise foi realizada utilizando dados reais de consumo, mensagens, chamadas, internet e faturamento de aproximadamente 500 clientes.

---

## Tecnologias Utilizadas

- Python
- Pandas
- NumPy
- Matplotlib
- SciPy
- Jupyter Notebook

---

## Etapas do Projeto

### Preparação dos Dados

- Tratamento e validação dos conjuntos de dados.
- Conversão de tipos de dados.
- Agregação mensal de utilização por usuário.
- Cálculo de receita individual considerando franquias e excedentes.

### Análise Exploratória

Avaliação de:

- Minutos consumidos
- Mensagens enviadas
- Uso de internet
- Receita mensal

Foram calculados:

- Média
- Variância
- Desvio padrão
- Distribuições dos dados

### Testes Estatísticos

Hipóteses avaliadas:

1. Existe diferença significativa entre a receita média dos planos Surf e Ultimate?
2. Existe diferença significativa entre a receita dos usuários da região NY-NJ e das demais regiões?

---

## Decisões de Limpeza e Processamento

### Chamadas com duração zero

Foram mantidas 26.834 chamadas com duração zero (aproximadamente 19,5% do total).

Decisão:
Essas chamadas foram consideradas registros válidos do sistema e mantidas na análise.

### Conversão de Dados

O consumo de internet foi convertido de MB para GB utilizando conversão binária:

- 1 GB = 1024 MB

### Agregação Mensal

O comportamento dos usuários foi consolidado mensalmente para análise de padrões de consumo e receita.

---

## Principais Descobertas

### Comportamento dos Usuários

Os usuários dos dois planos apresentaram padrões de utilização muito semelhantes:

| Métrica | Surf | Ultimate |
|----------|---------|-----------|
| Minutos Médios | 412 min | 410 min |
| Internet Média | 16,33 GB | 16,83 GB |

Conclusão:

O plano escolhido não altera significativamente o comportamento de consumo dos clientes.

---

### Receita

O plano Ultimate apresentou receita média aproximadamente 26% superior:

- Surf: US$ 57,29
- Ultimate: US$ 72,12

O teste estatístico indicou:

✅ p-value < 0,001

Portanto, existe diferença estatisticamente significativa entre os planos.

---

### Variabilidade Financeira

#### Plano Surf

- Desvio padrão: US$ 53,74

Alta variabilidade indica muitos clientes excedendo limites e gerando cobranças extras.

#### Plano Ultimate

- Desvio padrão: US$ 10,77

Receita mais previsível e estável.

---

### Análise Regional

Foi avaliada a região NY-NJ em comparação ao restante dos usuários.

Resultado:

✅ Não foi encontrada diferença estatisticamente significativa na receita.

- p-value = 0,082

Portanto, a localização geográfica não parece influenciar a receita.

---

## Recomendações de Negócio

### Priorizar o Plano Ultimate

Motivos:

- Maior receita média.
- Receita mais previsível.
- Menor variabilidade financeira.
- Melhor potencial para campanhas de aquisição.

### Revisar o Posicionamento do Plano Surf

O plano Surf apresentou:

- Alta variabilidade de faturamento.
- Maior dependência de cobranças por excedentes.
- Possível risco de insatisfação dos clientes devido aos limites mais restritivos.

### Segmentação Geográfica

Os resultados não justificam campanhas específicas para a região NY-NJ.

---

## Conclusão

A análise demonstrou que o plano Ultimate gera receita média significativamente superior ao plano Surf, mantendo maior estabilidade financeira.

Embora os clientes dos dois planos apresentem padrões de consumo muito semelhantes, o Ultimate produz resultados mais consistentes para o negócio.

Com base nos resultados estatísticos obtidos, a recomendação é direcionar estratégias de marketing e aquisição para o plano Ultimate.

---

## Competências Demonstradas

- Análise Estatística
- Testes de Hipótese
- Business Analytics
- Revenue Analysis
- Data Cleaning
- Exploratory Data Analysis (EDA)
- Data Visualization
- Tomada de Decisão Baseada em Dados
