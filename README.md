<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:0f172a,100:2563eb&height=190&section=header&text=Akash%20Siliveru&fontSize=48&fontColor=ffffff&animation=fadeIn&fontAlignY=36&desc=AI%20%2F%20ML%20Engineer%20%C2%B7%20LLM%20Apps%20%C2%B7%20Agentic%20Systems%20%C2%B7%20Applied%20ML&descAlignY=58&descSize=17" width="100%" />

<a href="https://github.com/akashsiliveru">
  <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=500&size=19&pause=1200&color=2563EB&center=true&vCenter=true&width=620&lines=Building+agentic+NL-to-SQL+pipelines;RAG+assistants+with+LangChain+%2B+ChromaDB;Classical+ML+from+EDA+to+deployed+app;Python+%C2%B7+FastAPI+%C2%B7+React+%C2%B7+SQL" alt="Typing SVG" />
</a>

<p>
  <a href="https://www.linkedin.com/in/akash-siliveru/"><img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" /></a>
  <a href="mailto:akashsiliveru1419@gmail.com"><img src="https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white" /></a>
  <a href="https://drive.google.com/file/d/1O7TZmedIcU0N5N-wCRL9igpoJQFGbfFu/view?usp=drive_link"><img src="https://img.shields.io/badge/Resume-4285F4?style=for-the-badge&logo=googledrive&logoColor=white" /></a>
  <img src="https://img.shields.io/badge/Hyderabad,%20India-111827?style=for-the-badge&logo=googlemaps&logoColor=white" />
</p>

</div>

---

## 👋 About me

I'm an **AI/ML engineer** who likes taking a model all the way to something people can use: an API, a dashboard, a chat box.

- 🤖 **LLM & agentic systems**: multi-agent NL-to-SQL with self-repair, retrieval-augmented assistants, schema-aware query planning
- 📊 **Applied ML**: imbalanced classification, NLP, recommendation, honest evaluation (precision / recall / F1, not just accuracy)
- 🛠️ **Full-stack delivery**: FastAPI backends, React + TypeScript frontends, Streamlit apps, PostgreSQL / MariaDB
- 🔎 **Data first**: every project starts with EDA, distribution checks and cleaning before any model

```python
akash = {
    "role":      "AI / ML Engineer",
    "focus":     ["LLM applications", "Agentic workflows", "RAG", "Applied ML"],
    "languages": ["Python", "SQL", "TypeScript"],
    "shipping":  ["FastAPI", "React", "Streamlit"],
    "location":  "Hyderabad, India",
    "open_to":   "AI / ML engineering roles",
}
```

---

## 🧰 Tech stack

<p align="center">
  <img src="https://skillicons.dev/icons?i=python,ts,react,vite,fastapi,postgres,mysql,sklearn,git,github,vscode&perline=12" />
</p>

| Area | Tools |
|---|---|
| **LLM / GenAI** | LangChain · Hugging Face Transformers · Sentence-Transformers · ChromaDB · OpenAI API · prompt engineering · RAG |
| **Agents & reasoning** | Multi-agent pipelines · schema graphs (NetworkX) · fuzzy matching (RapidFuzz) · SQL parsing & validation (sqlparse) |
| **Machine learning** | scikit-learn · imbalanced-learn (SMOTE, ADASYN, SMOTEENN) · GridSearchCV · RFECV · KNN · Random Forest · Naive Bayes |
| **NLP** | NLTK · TF-IDF · stemming & lemmatisation · language detection · machine translation |
| **Data** | Pandas · NumPy · SciPy (normality tests, skew / kurtosis) · Matplotlib · Seaborn · Plotly |
| **Backend & DB** | FastAPI · Pydantic · Uvicorn · PostgreSQL · MariaDB / MySQL |
| **Frontend & apps** | React · TypeScript · Vite · Recharts · ECharts · Streamlit |

---

## 🚀 Featured projects

### 🧠 Agentic SQL — natural language to safe SQL, with charts
**[agentic_sql_UI](https://github.com/akashsiliveru/agentic_sql_UI)** · Python · FastAPI · OpenAI · NetworkX · React + TypeScript

Ask an ERP database a business question in plain English and get validated SQL, the result, a chart and an insight. Built for ERP-scale schemas with hundreds of tables.

```text
Question → Intent → Metric resolver → Schema retriever → Join-graph resolver → Query planner
        → SQL generator → Validator ⟲ Repair loop → Read-only SQL gateway → Result validator
        → Insight agent + UI planner → chart in React
```

- **Agent pipeline** of 10 specialised agents with a **self-repair loop** when validation fails
- **Join paths** resolved over a schema graph built from foreign-key metadata (NetworkX)
- **Safe by design**: the gateway runs only `SELECT` / `WITH` and blocks every write and DDL statement
- **Business glossary and metric registry** so "unpaid vendor invoices" maps to the right tables and filters

---

### ⚖️ Nyay AI — multilingual legal assistant (RAG)
**[nyay-AI](https://github.com/akashsiliveru/nyay-AI)** · LangChain · ChromaDB · Hugging Face · TinyLlama · Streamlit

Helps Indian citizens understand which laws apply to their situation, in their own language.

- **Retrieval-augmented generation** over a legal corpus: PDF → chunking (700 / 100 overlap) → `all-MiniLM-L6-v2` embeddings → ChromaDB → top-k retrieval
- **Local LLM** (TinyLlama-1.1B-Chat) with a grounded prompt that answers only from retrieved law text
- **Multilingual**: detects the question's language, answers in English internally, translates the answer back

---

### 📈 SQL to UI — automatic chart selection for any query
**[sql_to_ui](https://github.com/akashsiliveru/sql_to_ui)** · FastAPI · PostgreSQL · React · TypeScript · Recharts

Run a SQL query and get the most suitable visual, picked automatically from the shape of the result.

- **Visualization selector** classifies columns as measures, dimensions or time and picks a KPI, table, pie, donut, bar or line chart
- Emits a **UI spec (JSON)** that a React renderer turns into the chart, so backend logic and rendering stay separate
- Unit tests for the selector logic

---

### 🍃 Arogya Plan — personalised diet recommendation
**[diet-recommendation-system](https://github.com/akashsiliveru/diet-recommendation-system)** · scikit-learn · imbalanced-learn · Streamlit · Plotly &nbsp;·&nbsp; [**🚀 Live demo**](https://diet-recommendation-system-2drzcfznrwqxxtr2ou6vny.streamlit.app/)

Predicts the right diet plan from a health profile (BMI, activity, blood sugar, cholesterol, goal).

- KNN classifier with scaling, **feature selection (RFECV / sequential)** and **GridSearchCV** tuning
- Compared **SMOTE, ADASYN and SMOTEENN** for class imbalance
- Deployed as a live Streamlit app with interactive Plotly charts

---

## 🧪 Machine learning & data projects

| Project | What it does | Approach | Result |
|---|---|---|---|
| [**Credit card fraud detection**](https://github.com/akashsiliveru/Credit-Card-Fraud-Detection) | Flags fraud in a dataset where only ~0.17% of transactions are fraud | Random Forest vs Decision Tree × oversampling, undersampling and SMOTE | Best: **RF + SMOTE**, precision **0.91**, recall **0.75**, F1 **0.82** on the fraud class |
| [**Fake news detection**](https://github.com/akashsiliveru/fake-news-detection) | Classifies news articles as fake or true | NLTK cleaning, stemming / lemmatisation, TF-IDF, Multinomial NB tuned with GridSearchCV | **~96.8% accuracy** |
| [**Stroke data EDA**](https://github.com/akashsiliveru/EDA-Stroke-Data) | Finds risk patterns in healthcare stroke data | Univariate / bivariate analysis, skew & kurtosis | Insight report |
| [**Penguins EDA**](https://github.com/akashsiliveru/Exploratory-Data-Analysis-Penguins) | Compares Palmer penguin species | Distributions, correlations, species profiles | Insight report |
| [**Tips EDA**](https://github.com/akashsiliveru/EDA-Project-On-Tips-Dataset) | What drives restaurant tipping | Normality tests (KS, Anderson-Darling), group comparisons | Insight report |
| [**Data manipulation with Pandas**](https://github.com/akashsiliveru/Data-manipulation-Using-Pandas) | Cleaning real datasets (Airbnb, IPL, Bengaluru housing, Audible…) | 500+ Pandas / NumPy problems across 6 datasets | Practice lab |

---

## 📊 GitHub stats

<p align="center">
  <img height="165" src="https://github-readme-stats.vercel.app/api?username=akashsiliveru&show_icons=true&hide_border=true&count_private=true&theme=transparent&title_color=2563eb&icon_color=2563eb" />
  <img height="165" src="https://github-readme-stats.vercel.app/api/top-langs/?username=akashsiliveru&layout=compact&hide_border=true&theme=transparent&title_color=2563eb" />
</p>

<p align="center">
  <img src="https://github-readme-activity-graph.vercel.app/graph?username=akashsiliveru&theme=minimal&hide_border=true&color=2563eb&line=2563eb&point=0f172a" width="95%" />
</p>

---

## 🌱 Currently

- Building **agent pipelines** that plan, validate and repair their own output
- Making RAG answers **grounded and evaluable**: retrieval quality, citations, refusals
- Taking ML projects from notebook to **API + UI + deployment**

---

<div align="center">

**Let's build something useful with AI.** &nbsp; [LinkedIn](https://www.linkedin.com/in/akash-siliveru/) · [Email](mailto:akashsiliveru1419@gmail.com) · [Resume](https://drive.google.com/file/d/1O7TZmedIcU0N5N-wCRL9igpoJQFGbfFu/view?usp=drive_link)

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:2563eb,100:0f172a&height=100&section=footer" width="100%" />

</div>
