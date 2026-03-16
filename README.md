# Previsão de Churn de Clientes — Projeto Completo de Machine Learning

![Python](https://img.shields.io/badge/Python-3.9+-blue)
![FastAPI](https://img.shields.io/badge/API-FastAPI-green)
![Streamlit](https://img.shields.io/badge/Dashboard-Streamlit-red)
![Machine Learning](https://img.shields.io/badge/ML-Scikit--Learn-orange)

## 📌 Visão Geral

Este projeto apresenta um **pipeline completo de Machine Learning** para **previsão de churn (cancelamento) de clientes**. Ele demonstra todo o ciclo de desenvolvimento de um produto de Data Science aplicado ao mundo real.

O projeto inclui:

* Análise exploratória de dados (EDA)
* Engenharia de features
* Treinamento de modelo de Machine Learning
* API de predição com **FastAPI**
* Dashboard interativo com **Streamlit**

O sistema permite treinar um modelo de previsão de churn, disponibilizar previsões através de uma API e visualizar insights por meio de um dashboard interativo.

---

# 🏗️ Arquitetura do Projeto

```
Dados → Análise Exploratória → Engenharia de Features → Treinamento do Modelo → API de Predição → Dashboard
```

Fluxo do projeto:

1. Carregamento e limpeza dos dados
2. Análise exploratória
3. Criação de variáveis para o modelo
4. Treinamento do modelo de churn
5. Disponibilização das previsões via API
6. Visualização dos resultados em dashboard

---

# 📂 Estrutura do Projeto

```
customer-churn-ml-v4
│
├── api
│   └── app.py              # API de predição com FastAPI
│
├── dashboard
│   └── app.py              # Dashboard interativo com Streamlit
│
├── data
│   └── cancelamentos.csv   # Dataset utilizado
│
├── src
│   ├── data_loader.py      # Carregamento de dados
│   ├── eda.py              # Análise exploratória
│   ├── features.py         # Engenharia de features
│   ├── train_model.py      # Treinamento do modelo
│   └── predict.py          # Lógica de predição
│
├── requirements.txt
└── README.md
```

---

# ⚙️ Instalação

Clone o repositório:

```bash
git clone https://github.com/YOUR_USERNAME/customer-churn-ml.git
cd customer-churn-ml
```

Instale as dependências:

```bash
pip install -r requirements.txt
```

---

# 🤖 Treinando o Modelo

Execute o pipeline de treinamento:

```bash
python src/train_model.py
```

Este processo irá:

* Carregar o dataset
* Aplicar engenharia de features
* Treinar o modelo de previsão de churn
* Salvar o modelo treinado

---

# 🚀 Executando a API de Predição

Inicie o servidor FastAPI:

```bash
uvicorn api.app:app --reload
```

A API estará disponível em:

```
http://127.0.0.1:8000
```

Documentação interativa da API:

```
http://127.0.0.1:8000/docs
```

---

# 📊 Executando o Dashboard

Para iniciar o dashboard interativo:

```bash
streamlit run dashboard/app.py
```

O dashboard permite:

* Visualizar estatísticas de churn
* Testar previsões
* Explorar insights do modelo

---

# 🧰 Tecnologias Utilizadas

* **Python**
* **Pandas**
* **NumPy**
* **Scikit-Learn**
* **FastAPI**
* **Streamlit**

---

# 💡 Possíveis Melhorias

Algumas melhorias que podem ser implementadas:

* Containerização com **Docker**
* Pipeline de **CI/CD**
* Monitoramento de modelo em produção
* Retreinamento automático
* Deploy em nuvem (AWS / GCP / Azure)

---

# 👨‍💻 Autor

Desenvolvido por **Afonso Alves**

GitHub: [https://github.com/afonso-alves-dev](https://github.com/afonso-alves-dev)

---

# 📜 Licença

Este projeto está sob a licença **MIT**.
