# Análise de Churn de Clientes — Módulo 15

## 📌 Sobre o projeto

Este projeto faz parte do exercício do **Módulo 15 — Análise: a segunda etapa da Pré-Modelagem**, do curso Profissão Cientista de Dados.

O objetivo é explorar uma base de clientes de uma empresa de telecomunicações para compreender o comportamento de **churn** (cancelamento de serviços), identificar possíveis outliers e investigar quais características dos clientes estão relacionadas aos cancelamentos.

A análise é realizada em Python, em um Jupyter Notebook, com estatísticas descritivas e visualizações gráficas.

## 🎯 Objetivos

- Realizar uma análise exploratória univariada dos dados.
- Examinar estatísticas descritivas das variáveis.
- Investigar possíveis valores atípicos (*outliers*).
- Visualizar a distribuição da variável-alvo `Churn`.
- Verificar o balanceamento de variáveis categóricas/booleanas.
- Realizar uma análise bivariada entre `Churn` e características dos clientes.
- Levantar variáveis potencialmente relevantes para compreender o cancelamento.

## 🧰 Tecnologias e bibliotecas

- **Python**
- **Pandas** — manipulação e análise de dados.
- **NumPy** — operações numéricas.
- **Matplotlib** — visualizações.
- **Seaborn** — recursos gráficos.
- **Plotly Express** — gráficos interativos.
- **Jupyter Notebook** — ambiente de execução.

## 📂 Arquivos

- `Profissao Cientista de Dados M15 Pratique (3).ipynb` — notebook com as etapas da análise e os gráficos.
- `CHURN_TELECON_MOD08_TAREFA_PART_02.csv` — base de dados esperada pelo notebook; deve estar no mesmo diretório do notebook.

> **Observação:** o CSV não está incorporado ao notebook. Para executar todas as células, disponibilize o arquivo `CHURN_TELECON_MOD08_TAREFA_PART_02.csv` no diretório de trabalho ou ajuste o caminho informado em `pd.read_csv()`.

## 🔎 Etapas da análise

### 1. Carregamento dos dados

A base CSV é carregada com Pandas e inspecionada inicialmente para visualizar os registros.

### 2. Análise univariada

São examinadas estatísticas descritivas e distribuições de variáveis, incluindo:

- `Churn`
- `Total_Pago`
- `Tempo_como_Cliente`
- `Pagamento_Mensal`

Também são construídos gráficos de contagem para variáveis como gênero, faixa etária (`Idoso`), estado civil (`Casado`), dependentes, serviços contratados, tipo de contrato e método de pagamento.

### 3. Investigação de outliers

O notebook utiliza estatísticas descritivas e *boxplots* para investigar possíveis valores atípicos. A atividade propõe identificar e tratar as colunas com outliers, justificando a decisão tomada.

### 4. Análise bivariada

São exploradas relações entre `Churn` e as seguintes variáveis:

- `Dependentes`
- `Servico_Internet`
- `Servico_Seguranca`
- `Suporte_Tecnico`
- `Tipo_Contrato`

Os histogramas agrupados permitem comparar a distribuição de cancelamentos entre as categorias dessas variáveis.

## 📊 Principais observações registradas no notebook

De acordo com as respostas documentadas no próprio exercício:

- Aproximadamente **26% dos clientes** cancelaram o serviço.
- `Total_Pago` foi apontada como uma variável que merecia investigação de possíveis outliers, devido à diferença entre média e mediana.
- A análise de balanceamento indicou `Casado` e `Genero` como as variáveis consideradas balanceadas no exercício.
- Na análise bivariada, `Dependentes`, `Servico_Internet`, `Servico_Seguranca`, `Suporte_Tecnico` e `Tipo_Contrato` foram destacadas como variáveis potencialmente importantes para estudar o churn.
- O notebook sugere que os resultados podem ajudar a direcionar campanhas de retenção para perfis de clientes com maior ocorrência de cancelamento.

Essas observações refletem as respostas registradas no exercício e devem ser interpretadas no contexto da base analisada. Associação entre variáveis, por si só, não demonstra causalidade.

## ⚙️ Como executar

1. Clone ou baixe este repositório.
2. Coloque o arquivo CSV `CHURN_TELECON_MOD08_TAREFA_PART_02.csv` no mesmo diretório do notebook.
3. Instale as bibliotecas necessárias:

   ```bash
   pip install pandas numpy matplotlib seaborn plotly jupyter
   ```

4. Inicie o Jupyter Notebook:

   ```bash
   jupyter notebook
   ```

5. Abra `Profissao Cientista de Dados M15 Pratique (3).ipynb` e execute as células em ordem.

## 🚧 Limitações e próximos passos

- Completar a etapa de identificação e tratamento de outliers, documentando os critérios e as justificativas.
- Explorar outras relações entre variáveis e `Churn`.
- Complementar as comparações com taxas percentuais por categoria, evitando conclusões baseadas apenas em contagens absolutas.
- Em uma etapa futura, preparar os dados para modelagem preditiva, caso esse seja o objetivo do projeto.

## 📚 Contexto

Exercício acadêmico do curso **Profissão Cientista de Dados — Módulo 15**.

---

*Projeto desenvolvido para fins de estudo e prática de análise exploratória de dados.*
