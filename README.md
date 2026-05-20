# Análise Exploratória de Dados – Sample Superstore


**Autor:** Daniela dos Anjos  
**Curso:** Introdução ao Data Science – Carreira Tech (SCTEC)  
**Data:** Maio/2026  
**Contato:** oidanianjos@gmail.com
**LinkedIn:** https://www.linkedin.com/in/daniela-anjos/
**GitHub:** https://github.com/d-anjos/


---


##  Sobre o Projeto


Este projeto consiste em uma Análise Exploratória de Dados (AED) do dataset *Sample Superstore*, disponível publicamente no Kaggle. O objetivo é compreender o comportamento de vendas, lucro, impacto dos descontos e desempenho por categoria/segmento, gerando insights acionáveis para uma rede varejista americana.


---


##  Ferramentas Utilizadas


- **Python 3** + Google Colab
- **Bibliotecas:** pandas, numpy, matplotlib, seaborn
- **Visualização de dados:** Looker Studio (dashboard interativo)
- **Controle de versão:** Git + GitHub


---


##  Estrutura do Projeto


Daniela_Anjos_Desafio_Extra_DataScience.zip
│
├── Daniela_Anjos_Desafio_Extra_DataScience.ipynb # Notebook principal
├── Sample_Superstore.csv # Dataset original
├── visualizacoes/ # Gráficos gerados (.png)
│    ├──boxplot_outliers.png
│    ├──desconto_lucro_subcategorias_deficitarias.png
│    ├──desconto_lucro_subcategorias_lucrativas.png
│    ├──desconto_vs_lucro.png
│    ├──outliers_com_limites.png
│    ├──tendencia_vendas_lucro.png
│    ├──top10_clientes_lucro.png
│    ├──vendas_lucro_por_subcategoria_por_lucro.png
│    ├──vendas_mensais_por_categoria.png
│    ├──vendas_mensais_por_segmento.png
│    ├──vendas_por_categoria.png
│    └──vendas_por_segmento.png
└── Daniela_Anjos_Dashboard.pdf # Versão estática do dashboard
├── Daniela_Anjos_documentacao.txt # Documentação completa do projeto
└── README.md # Este arquivo


---


##  Como Executar o Projeto


### 1. No Google Colab (recomendado)
- Acesse o [link do notebook](https://colab.research.google.com/drive/1jOEQQIPmq-Xvv4X6w1gjWUOdwYNoikUK?usp=drive_link).
- No menu, clique em **“Copiar para o Drive”** para salvar uma cópia editável.
- Execute as células em ordem (Runtime → Run all).
- O dataset é carregado via upload manual (basta selecionar o arquivo `Sample_Superstore.csv`).


### 2. Localmente (Python + Jupyter)
```bash
# Clone o repositório
git clone https://github.com/d-anjos/d-anjos-Daniela_Anjos_Desafio_DataScience.git


# Instale as dependências
pip install pandas numpy matplotlib seaborn


# Execute o Jupyter Notebook
jupyter notebook Daniela_Anjos_Desafio_DataScience.ipynb




###  Principais Insights


Tecnologia é a categoria mais lucrativa – mesmo com vendas ligeiramente menores que Móveis, seu lucro é 7x maior.


Descontos acima de 20% geram prejuízo – a relação é fortemente negativa, especialmente para subcategorias como Tables, Bookcases e Supplies.


Sazonalidade acentuada – picos de vendas em novembro/dezembro, mas o lucro não acompanha na mesma proporção (sugere descontos agressivos ou aumento de custos).


Segmento Consumer domina – representa ~50% das vendas, com comportamento mais volátil; Corporate e Home Office são mais estáveis.


Modo de envio – Standard Class dá maior lucro total (pelo volume), mas First Class tem a maior lucratividade média por transação.


Base concentrada – os 10 maiores clientes representam uma parcela significativa do lucro total, indicando a importância de estratégias de fidelização.


## Decisões Técnicas Relevantes
Valores nulos e duplicatas: verificados e nenhum foi encontrado.


Conversão de tipos: Order ID, Customer ID e Postal Code transformados em string (identificadores). Datas convertidas para datetime.


Outliers: identificados via IQR, mas não removidos para preservar a realidade dos dados; apenas adicionadas linhas de referência nos boxplots.


Tradução das colunas: nomes originais em inglês foram mantidos nas etapas de exploração inicial e depois traduzidos para português, facilitando a legibilidade do notebook.


Gráficos: escolha de tipos adequados para cada pergunta de negócio (dispersão para relação desconto×lucro, barras para comparação de categorias, linhas para séries temporais).




##  Tecnologias Utilizadas
Python 3.10+


Pandas – manipulação e limpeza de dados


NumPy – operações matemáticas e arrays


Matplotlib & Seaborn – visualização de dados


Google Colab – ambiente de desenvolvimento


Looker Studio – dashboard interativo


Git & GitHub – versionamento e portfólio




##  Links Úteis


Dashboard interativo (Looker Studio):
https://datastudio.google.com/reporting/7e2ca710-5de2-4466-9623-fcadd0ad8ff5


Repositório GitHub:
https://github.com/d-anjos/d-anjos-Daniela_Anjos_Desafio_DataScience


Dataset original (Kaggle):
Sample Superstore Dataset
https://www.kaggle.com/datasets/vivek468/superstore-dataset-final


##  Observações


Todos os outliers foram identificados mas não removidos, pois representam transações reais e sua exclusão poderia introduzir viés.


As colunas foram renomeadas para português para facilitar a interpretação.


O código está comentado e as decisões técnicas estão justificadas na documentação.


##  Licença


Este projeto é de uso educacional, parte do programa SCTEC – Carreira Tech.