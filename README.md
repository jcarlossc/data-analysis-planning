# 📌 ETAPAS DO PLANEJAMENTO DA ANÁLISE DE DADOS

O planejamento é a fase estratégica do projeto, onde são definidos 
os propósitos do projeto: 

- o que será feito,
- por que,
- como,
- e com quais recursos.

Serve para garantir que o trabalho de análise seja direcionado, 
eficiente e gere valor real.

---

## 📌 1. Definição do problema (ou questão de pesquisa)
**Objetivo:** compreender claramente o que se quer resolver ou descobrir.
o ponto de partida de todo o projeto.

**Perguntas-chave:**
- Que problema motivou esta análise?
- Qual decisão depende desses dados?
- Existe uma hipótese a ser testada?

**Exemplo:**
"Por que o número de clientes que cancelam o serviço aumentou nos últimos meses?"

---

## 📌 2. Definição dos objetivos e metas da análise
**Objetivo:** transformar o problema em objetivos específicos e mensuráveis.
Os objetivos determinam o foco e os critérios de sucesso.

**Perguntas-chave:**
- O que exatamente queremos medir, prever ou explicar?
- Quais métricas indicam sucesso?
- Quais resultados esperamos obter?

**Exemplo:**
"Identificar os principais fatores que influenciam o cancelamento e prever 
a probabilidade de churn de cada cliente com 85% de acurácia."

---

## 📌 3. Definição do escopo e das entregas
**Objetivo:** delimitar o que está dentro e fora do projeto, para evitar retrabalho e dispersão.

**Inclui:**
- Escopo funcional (quais análises, variáveis ou períodos serão considerados)
- Escopo temporal (prazo para cada etapa)
- Entregáveis (relatório, dashboard, modelo, insights etc.)

**Exemplo:**
"A análise abrangerá clientes ativos nos últimos 12 meses e resultará em um relatório PDF e um dashboard interativo no Power BI."

---

## 📌 4. Identificação das fontes de dados</h2>
**Objetivo:** determinar onde os dados estão, quem os fornece e como serão obtidos.

**Perguntas-chave:**
- Os dados já existem ou precisarão ser coletados?
- Estão em planilhas, bancos de dados, APIs ou sistemas externos?
- Há restrições de acesso, privacidade ou LGPD?

**Exemplo:**
"Usar dados internos de CRM e transações, e dados externos do IBGE para perfil 
socioeconômico das regiões."

---

## 📌 5. Planejamento da coleta e integração dos dados</h2>
**Objetivo:** descrever como os dados serão coletados, integrados e armazenados.
Essa etapa garante que, ao iniciar a análise, as fontes estejam acessíveis e consistentes.

**Itens a definir:**
- Métodos de coleta (API, web scraping, exportação, query SQL, formulários etc.)
- Periodicidade (dados históricos, semanais, em tempo real)
- Ferramentas (Python, Pandas, Requests, Airflow etc.)
- Padrões de nomeação e armazenamento (pasta /data/raw, /data/processed etc.)

**Exemplo:**
Coletar dados de vendas do banco PostgreSQL via SQLAlchemy e salvar em formato .csv 
na pasta /data/raw.

---

## 📌 6. Planejamento da estrutura e preparação dos dados</h2>
**Objetivo:** antecipar como os dados serão organizados e tratados para análise.

**Inclui:**
- Definição de variáveis relevantes
- Padronização de formatos (datas, valores monetários, strings)
- Estratégias para lidar com valores ausentes, duplicados ou outliers
- Modelagem de tabelas (se for necessário juntar várias fontes)

**Exemplo:**
"Remover duplicatas, padronizar colunas de datas no formato ISO e imputar valores 
faltantes de renda pela mediana."

---

## 📌 7. Definição das técnicas analíticas e estatísticas</h2>
**Objetivo:** planejar como os dados serão analisados e quais métodos serão utilizados.

**Possíveis métodos:**
- Estatística descritiva (médias, dispersão, percentis)
- Análise exploratória (correlações, histogramas, boxplots)
- Modelos preditivos (regressão, classificação)
- Agrupamentos (clusterização)
- Séries temporais
- Análises geográficas

**Exemplo:**
"Aplicar regressão logística para prever churn e análise de correlação para identificar 
variáveis mais influentes."

---

## 📌 8. Definição das ferramentas e tecnologias</h2>
**Objetivo:** escolher o conjunto de ferramentas adequadas ao escopo e à equipe.

**Critérios:**
- Linguagem (Python, R, SQL, etc.)
- Bibliotecas (Pandas, Scikit-Learn, Seaborn, etc.)
- Ambiente de execução (Jupyter, VSCode, Google Colab)
- Controle de versão (Git/GitHub)
- Armazenamento e visualização (Power BI, Looker, Dash, Streamlit)

**Exemplo:**
"Usar Python (Pandas + Scikit-Learn) para análise e Power BI para visualização final."

---

## 📌 9. Definição das métricas de avaliação</h2>
**Objetivo:** definir como medir o sucesso da análise e dos resultados gerados.

**Métricas comuns:**
- Modelos preditivos: Acurácia, F1-Score, RMSE
- Desempenho do processo: tempo de execução, cobertura de dados
- Impacto de negócio: aumento de vendas, redução de custos, taxa de retenção

**Exemplo:**
"O modelo será considerado satisfatório se atingir F1-Score acima de 0.80 e explicar 
pelo menos 70% da variância dos dados."

---

## 📌 10. Cronograma e responsabilidades</h2>
**Objetivo:** organizar quem faz o quê e em quanto tempo.

**Inclui:**
- Divisão de tarefas por função (analista, cientista de dados, engenheiro, gestor)
- Estimativa de duração de cada etapa
- Dependências entre tarefas
- Ferramentas de acompanhamento (Trello, Jira, Notion, etc.)

**Exemplo de cronograma simplificado:**
| Etapas | Responsável | Prazos |
| ------ | ----------- | ------ |
| Coleta e limpeza dos dados | Analista de Dados | Semana 1 |
| Análise exploratória | Cientista de Dados | Semana 2 |
| Modelagem e validação | Cientista de Dados | Semana 3 |
| Visualização e relatório final | Analista de BI | Semana4 |

---

## 📌 11. Planejamento da documentação e comunicação</h2>
**Objetivo:** garantir que o projeto seja compreensível, reprodutível e comunicável.

**Inclui:**
- Documentar decisões, métodos e hipóteses
- Criar README do projeto
- Planejar relatórios e apresentações para stakeholders
- Definir formato de entrega (PDF, dashboard, notebook, etc.)

**Exemplo:**
"Gerar relatório final em PDF com gráficos e recomendações, e disponibilizar notebook Jupyter no GitHub com instruções de execução."

---

