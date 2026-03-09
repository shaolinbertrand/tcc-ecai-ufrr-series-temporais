🚌 TranspoPredict: ML Demand Forecasting for Road Transport

Atenção: Este repositório contém o código-fonte desenvolvido para o Trabalho de Conclusão de Curso (TCC) da Especialização em Inteligência Artificial Aplicada à Indústria 4.0 pela Universidade Federal de Roraima (UFRR).

📖 Sobre o Projeto / About the Project

Este projeto implementa uma arquitetura de Machine Learning baseada em métodos Ensemble (Random Forest e LightGBM) para prever a procura diária de passagens no transporte rodoviário interestadual na região Amazónica.

O foco principal é a transição de um modelo de gestão reativo para um modelo orientado a dados (Data-Driven), mitigando os riscos de alocação ineficiente de frota e reduzindo custos operacionais. Além do modelo matemático, o projeto inclui o desenvolvimento de um Dashboard Interativo com regras de negócio embutidas para proteger a operação logística.

✨ Principais Funcionalidades / Key Features

Análise Comparativa de Algoritmos: Avaliação rigorosa entre Regressão Linear (Baseline), Random Forest e LightGBM usando a métrica RMSE.

Engenharia de Atributos Avançada: Tratamento de sazonalidade cíclica utilizando transformações trigonométricas (seno/cosseno) para dias do ano e da semana.

Lags Temporais Dinâmicos: Incorporação de memória temporal para captar tendências de curtíssimo e longo prazo.

Dashboard Clean (UX Otimizado): Interface desenvolvida com ipywidgets e matplotlib, permitindo a visualização da estimativa através de gráficos dinâmicos (Barras, Linhas, Pirulito).

Mecanismo de Segurança (Arranque a Frio): O painel avalia a latência dos dados. Se detetar a falta de histórico recente (ex: a rota esteve inoperante), o sistema bloqueia a inferência puramente estatística e emite um alerta de segurança, exigindo o julgamento humano.

📸 Capturas de Ecrã / Screenshots

!
Interface de previsão otimizada com validação de status de dados em tempo real.

🛠️ Tecnologias Utilizadas / Tech Stack

Linguagem: Python

Manipulação de Dados: Pandas, NumPy, SQLAlchemy

Machine Learning: Scikit-Learn (Random Forest, Linear Regression), LightGBM

Visualização & UI: Matplotlib, ipywidgets

Ambiente: Jupyter Notebook / Google Colab

🔒 Aviso sobre os Dados (Data Disclaimer)

Por questões de conformidade com a Lei Geral de Proteção de Dados (LGPD) e respeito ao sigilo industrial da empresa parceira (AMATUR), os dados reais de vendas não estão incluídos neste repositório.

O ficheiro dataset_mock.csv fornecido contém dados inteiramente fictícios/anonimizados, criados exclusivamente para demonstrar o funcionamento da interface e do pipeline de previsão.

🚀 Como Executar / How to Run

Clone o repositório:

git clone [https://github.com/shaolinbertrand/tcc-ecai-ufrr-series-temporais.git](https://github.com/shaolinbertrand/tcc-ecai-ufrr-series-temporais.git)


Instale as dependências:

pip install -r requirements.txt


Execute o Notebook:

jupyter notebook TCC.ipynb


👨‍💻 Autor / Author

Jean Bertrand Paixão da Silva

Cientista da Computação & Especialista em IA Aplicada à Indústria 4.0

Professor Substituto no Departamento de Ciência da Computação (UFRR)

LinkedIn | Lattes

Desenvolvido em Boa Vista, Roraima, Brasil - 2025.
