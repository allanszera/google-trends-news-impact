# Google Trends x Notícias: Análise de Impacto

Projeto de Engenharia de Dados e Análise, da **extração à visualização**, para investigar como notícias influenciam tendências de busca no Google Brasil.

---

## ✨ Objetivo

Extrair dados do Google Trends e portais de notícias, consolidar em um Data Warehouse, aplicar transformações (ETL) e criar dashboards interativos para analisar correlações entre as notícias do dia e as buscas mais populares.

---

## 🛠️ Stack Utilizada

* **Python** (pandas, requests, BeautifulSoup, feedparser, playwright/selenium)
* **Banco de Dados**: PostgreSQL (ou SQLite para prototipação)
* **Dashboard**: Streamlit ou Power BI
* **Versionamento**: Git/GitHub

---

## 📁 Estrutura de Pastas

```
google-trends-news-impact/
│
├── data/                 # Dados brutos e processados
│   ├── raw/
│   └── processed/
├── etl/                  # Scripts de extração e transformação
│   ├── extract_trends.py
│   ├── extract_news.py
│   └── transform_load.py
├── dw/                   # Scripts de criação do banco/modelo
│   └── create_tables.sql
├── dashboard/            # Código do dashboard
│   └── app.py
├── notebooks/            # Notebooks exploratórios
├── requirements.txt
├── README.md
└── .gitignore
```

---

## 🚀 Como rodar o projeto

1. **Clone o repositório:**

   ```bash
   git clone https://github.com/allanszera/google-trends-news-impact.git
   cd google-trends-news-impact
   ```

2. **Crie o ambiente virtual:**

   ```bash
   python -m venv .venv
   source .venv/bin/activate  # Linux/Mac
   .venv\Scripts\activate     # Windows
   ```

3. **Instale as dependências:**

   ```bash
   pip install -r requirements.txt
   ```

4. **Execute os scripts de extração:**

   ```bash
   python etl/extract_trends.py
   python etl/extract_news.py
   ```

5. **Transforme e carregue os dados:**

   ```bash
   python etl/transform_load.py
   ```

6. **Execute o dashboard:**

   ```bash
   streamlit run dashboard/app.py
   ```

---

## 📊 Etapas do Projeto

1. **Extração**

   * Coleta de trending topics do Google Trends (via CSV, RSS ou scraping dinâmico)
   * Coleta de manchetes de notícias (G1, BBC, CNN, Google News RSS)
2. **Armazenamento**

   * Estrutura de Data Warehouse simples para integração dos dados
3. **Transformação**

   * Limpeza, padronização, enriquecimento e cruzamento das informações
4. **Dashboard**

   * Visualização das correlações e insights
5. **Documentação**

   * Processo documentado aqui e com notebooks passo a passo

---

## 📝 To-do (checklist)

* [ X ] Montar estrutura de pastas e arquivos iniciais
* [ ] Implementar extração dos dados do Trends
* [ ] Implementar extração das notícias
* [ ] Criar banco e modelo relacional
* [ ] ETL: Transformação e carga no DW
* [ ] Dashboard e análise exploratória
* [ ] Documentação completa do processo

---

## 📄 Licença

Projeto com fins educacionais. Respeite sempre as políticas de uso das fontes e a LGPD.

---

## 🤝 Contribuição

Pull Requests são bem-vindos! Sugestões, melhorias e dúvidas, use as [issues](https://github.com/allanszera/google-trends-news-impact/issues).

---

## 📫 Contato

Dúvidas? Fale comigo no [LinkedIn](https://www.linkedin.com/in/allanszera/).
