<h1 align="center">Hi, I'm Prakruthi Manjunath</h1>

<h3 align="center">
Data Engineer | Azure | Databricks | PySpark | SQL | Python
</h3>

<p align="center">
<img src="https://readme-typing-svg.herokuapp.com?font=Poppins&size=24&duration=3000&pause=1000&color=0E75B6&center=true&vCenter=true&width=700&lines=Data+Engineer;Building+Scalable+Data+Pipelines;Azure+%7C+Databricks+%7C+PySpark;Open+to+Data+Engineering+Opportunities" />
</p>

## About Me

-  MSc Data Science - University of Surrey
-  Data Engineer with 3+ years of experience
-  Currently Data Administrator at the University of Surrey
-  Passionate about Azure, Databricks, PySpark & Cloud Data Engineering
-  Currently preparing for Databricks Data Engineer Associate
-  Open to Data Engineering opportunities in the UK

##  Featured Projects

### [AI News Insights](https://github.com/Prakruthimanjunath20/ai-news-insights)
`Python` `FastAPI` `scikit-learn` `Pydantic` `Claude API` `GitHub Actions`

Turns a stream of financial headlines into deduplicated stories, with the companies,
sector, regulator and sentiment of each story and the UK stocks most likely to be affected.

- Groups the same event reported by different outlets using character n-gram TF-IDF,
  a 72-hour time window and union-find
  ([commit](https://github.com/Prakruthimanjunath20/ai-news-insights/commit/0ac9890375121b69e5c240ac8e591153759ca367))
- Enriches stories offline with a finance sentiment lexicon, or with Claude through
  structured tool use, falling back to the rules if an API call fails
  ([commit](https://github.com/Prakruthimanjunath20/ai-news-insights/commit/34b400c6b14918f253a9dcab789d9b4b184a675d))
- Async RSS ingestion, entity-aware search and watch-list alerts behind a FastAPI
  service, web page and CLI
  ([commit](https://github.com/Prakruthimanjunath20/ai-news-insights/commit/3c90029512669a8c7f6cf06a3c14616f03c6a481))
- 28 tests, with CI on Python 3.11–3.13

### [dev-productivity-mcp](https://github.com/Prakruthimanjunath20/dev-productivity-mcp)
`Python` `MCP` `httpx` `Pydantic` `GitHub REST API`

An MCP server that gives AI assistants such as Claude read-only tools for git
repositories: repo overviews, standup reports, changelogs, TODO scans, branch health
and pull request summaries.

- Seven typed tools and two prompts built on the MCP Python SDK 2.x
  ([commit](https://github.com/Prakruthimanjunath20/dev-productivity-mcp/commit/1845f5e20e01310b4502beefc814daa93832d54f))
- Folder allow-list and a git runner that refuses option-like input
  ([commit](https://github.com/Prakruthimanjunath20/dev-productivity-mcp/commit/a58c4d0cfa573c07a7aed38f985d4ce2de5d951f))
- 23 tests, including end-to-end calls through a real MCP client

### [repo-rag-assistant](https://github.com/Prakruthimanjunath20/repo-rag-assistant)
`Python` `RAG` `BM25` `Claude API` `FastAPI`

Ask questions about any GitHub repository and get answers grounded in its code, with
every claim cited to a file and line range.

- Chunks Python by function, class and method using `ast`, and retrieves with BM25
  over a code-aware tokenizer
  ([commit](https://github.com/Prakruthimanjunath20/repo-rag-assistant/commit/fb21074366857f1da51ece15ca9de826e8c12183))
- Claude answers only from numbered sources; every citation is checked against what
  was retrieved, and uncited answers are flagged
  ([commit](https://github.com/Prakruthimanjunath20/repo-rag-assistant/commit/5b3c81a81dae9b12e9f8dc2dc47d69c6acbfb0a7))
- Retrieval eval set run in CI: recall@5 = 1.00, MRR = 0.79
  ([commit](https://github.com/Prakruthimanjunath20/repo-rag-assistant/commit/7f2d324b843a5566e6efb4069d716f301c3d0523))

### [guarded-agent](https://github.com/Prakruthimanjunath20/guarded-agent)
`Python` `AI agents` `Claude tool use` `Pydantic`

A tool-using Claude agent with guardrails: typed tools, human approval for side
effects, step and call budgets, prompt-injection flags, and replayable JSONL traces.

- Tool schemas generated from type hints, with argument validation errors returned
  to the model ([commit](https://github.com/Prakruthimanjunath20/guarded-agent/commit/e54b83591d5d2fe35edcafe784b9186a6a770ff3))
- Policy layer for allow-lists, approvals, budgets and injection detection
  ([commit](https://github.com/Prakruthimanjunath20/guarded-agent/commit/417ad38330adcd12910a072e497af874784f112d))
- Offline demo where a planted injection is flagged and the email it asks for is denied

### [llm-eval-harness](https://github.com/Prakruthimanjunath20/llm-eval-harness)
`Python` `LLM evaluation` `LLM-as-judge` `GitHub Actions`

Regression tests for LLM apps: YAML suites, rule and similarity checks, Claude as a
judge, repeated runs to measure flakiness, and a baseline gate that fails CI on
regressions.

- Claude judge with structured verdicts through a forced tool call
  ([commit](https://github.com/Prakruthimanjunath20/llm-eval-harness/commit/171204c914b040058f60a02fb9847a7cc9dc0fd1))
- Parallel, repeated runs with per-case pass rates
  ([commit](https://github.com/Prakruthimanjunath20/llm-eval-harness/commit/27e3b63ce2904e8d6cd2e2a43b0cda3320f1dc63))
- CI gate and Markdown summary on the GitHub Actions run page
  ([commit](https://github.com/Prakruthimanjunath20/llm-eval-harness/commit/8ca2d53d84531ea93373b33c54db528cbd8bdea9))

### [abbreviation-detector](https://github.com/Prakruthimanjunath20/abbreviation-detector)
`Python` `NLP` `CRF` `sequence labelling` `FastAPI`

Finds abbreviations and their long forms in scientific text and links them, trained
on the PLOD dataset (about 160k sentences).

- CRF tagger stacked with the Schwartz-Hearst rule algorithm: **0.766 span F1** on
  held-out papers, against 0.486 for the rules alone
  ([commit](https://github.com/Prakruthimanjunath20/abbreviation-detector/commit/dfc13b5481a77979b89777481dc1c69f143751ec))
- Tokenizer fix that raised the achievable ceiling from 0.89 to 0.96 F1, and
  regularisation that halved the model size while improving accuracy
  ([commit](https://github.com/Prakruthimanjunath20/abbreviation-detector/commit/36fd1e90ccd97e62996a093f7a57287c8c3a94d5))

##  Team Projects

### [Farmers Local Market](https://github.com/shashanksuresh18/farmers_local_market)
`Python` `Flask` `Flask-SQLAlchemy` `Flask-Login` `Docker`

MSc group project at the University of Surrey (2024): a web marketplace connecting
local farmers' market vendors with customers, built by a team of six.

- **My contribution:** the vendor and product features of the Flask back end: vendor
  home and profile editing, adding, editing and listing products, product detail and
  review pages, and the market and product listings
  ([commit](https://github.com/shashanksuresh18/farmers_local_market/commit/bf12f8930262c107e5395157663ad6a447f34535))

##  Certifications

![AZ-900](https://img.shields.io/badge/AZ--900-Azure%20Fundamentals-0078D4?style=for-the-badge&logo=microsoftazure&logoColor=white)

![DP-900](https://img.shields.io/badge/DP--900-Azure%20Data%20Fundamentals-0078D4?style=for-the-badge&logo=microsoftazure&logoColor=white)

![Databricks](https://img.shields.io/badge/Databricks-Data%20Engineer%20Associate%20(In%20Progress)-EF3E42?style=for-the-badge&logo=databricks&logoColor=white)

##  Contribution Graph

[![Prakruthi's github activity graph](https://github-readme-activity-graph.vercel.app/graph?username=Prakruthimanjunath20&theme=tokyo-night)](https://github.com/ashutosh00710/github-readme-activity-graph)

##  Connect With Me

<p align="left">

<a href="https://www.linkedin.com/in/prakruthi21">
<img src="https://img.shields.io/badge/LinkedIn-blue?style=for-the-badge&logo=linkedin"/>
</a>

<a href="mailto:prakruthimanjunath20@gmail.com">
<img src="https://img.shields.io/badge/Gmail-red?style=for-the-badge&logo=gmail"/>
</a>

</p>

![](https://komarev.com/ghpvc/?username=Prakruthimanjunath20&style=for-the-badge)

##  Tech Stack

<p align="left">
  <img src="https://skillicons.dev/icons?i=python,fastapi,azure,git,github,githubactions,docker,vscode,aws,mysql,postgres" />
</p>


<p align="left">
  <img src="https://img.shields.io/badge/Databricks-EF3E42?style=for-the-badge&logo=databricks&logoColor=white"/>
  <img src="https://img.shields.io/badge/Snowflake-29B5E8?style=for-the-badge&logo=snowflake&logoColor=white"/>
  <img src="https://img.shields.io/badge/PySpark-E25A1C?style=for-the-badge&logo=apachespark&logoColor=white"/>
  <img src="https://img.shields.io/badge/Airflow-017CEE?style=for-the-badge&logo=apacheairflow&logoColor=white"/>
</p>
