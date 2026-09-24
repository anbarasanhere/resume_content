\documentclass[letterpaper,11pt]{article}

\usepackage{latexsym}
\usepackage[empty]{fullpage}
\usepackage{titlesec}
\usepackage{marvosym}
\usepackage[usenames,dvipsnames]{color}
\usepackage{verbatim}
\usepackage{enumitem}
\usepackage[hidelinks]{hyperref}
\usepackage{fancyhdr}
\usepackage[english]{babel}
\usepackage{tabularx}
\usepackage{hyphenat}
\usepackage{fontawesome}
\input{glyphtounicode}


%---------- FONT OPTIONS ----------
% sans-serif
% \usepackage[sfdefault]{FiraSans}
% \usepackage[sfdefault]{roboto}
% \usepackage[sfdefault]{noto-sans}
% \usepackage[default]{sourcesanspro}

% serif
% \usepackage{CormorantGaramond}
% \usepackage{charter}


\pagestyle{fancy}
\fancyhf{} % clear all header and footer fields
\fancyfoot{}
\renewcommand{\headrulewidth}{0pt}
\renewcommand{\footrulewidth}{0pt}

% Adjust margins
\addtolength{\oddsidemargin}{-0.5in}
\addtolength{\evensidemargin}{-0.5in}
\addtolength{\textwidth}{1in}
\addtolength{\topmargin}{-.5in}
\addtolength{\textheight}{1.0in}

\urlstyle{same}

\raggedbottom
\raggedright
\setlength{\tabcolsep}{0in}

% Sections formatting
\titleformat{\section}{
  \vspace{-10pt}\scshape\raggedright\large
}{}{0em}{}[\color{black}\titlerule \vspace{-5pt}]

% Ensure that generate pdf is machine readable/ATS parsable
\pdfgentounicode=1

%-------------------------
% Custom commands

\newcommand{\resumeItem}[1]{
  \item\small{
    {#1 \vspace{-2pt}}
  }
}

\newcommand{\resumeSubheading}[4]{
  \vspace{-2pt}\item
    \begin{tabular*}{0.97\textwidth}[t]{l@{\extracolsep{\fill}}r}
      \textbf{#1} & #2 \\
      \textit{\small#3} & \textit{\small #4} \\
    \end{tabular*}\vspace{-7pt}
}


\newcommand{\resumeSubSubheading}[2]{
    \vspace{-2pt}\item
    \begin{tabular*}{0.97\textwidth}{l@{\extracolsep{\fill}}r}
      \textit{\small#1} & \textit{\small #2} \\
    \end{tabular*}\vspace{-10pt}
}


\newcommand{\resumeEducationHeading}[4]{
  \vspace{-10pt}\item
    \begin{tabular*}{0.97\textwidth}[t]{l@{\extracolsep{\fill}}r}
      \textbf{#1} & #2 \\
      \textit{\small#3} & \textit{\small #4} \\
      \textit{\small#5} & \textit{\small #6} \\
    \end{tabular*}\vspace{-10pt}
}


\newcommand{\resumeProjectHeading}[2]{
    \vspace{-2pt}\item
    \begin{tabular*}{0.97\textwidth}{l@{\extracolsep{\fill}}r}
      \small#1 & #2 \\
    \end{tabular*}\vspace{-7pt}
}


\newcommand{\resumeOrganizationHeading}[4]{
  \vspace{-2pt}\item
    \begin{tabular*}{0.97\textwidth}[t]{l@{\extracolsep{\fill}}r}
      \textbf{#1} & \textit{\small #2} \\
      \textit{\small#3}
    \end{tabular*}\vspace{-7pt}
}

\newcommand{\resumeSubItem}[1]{\resumeItem{#1}\vspace{-4pt}}

\renewcommand\labelitemii{$\vcenter{\hbox{\tiny$\bullet$}}$}

\newcommand{\resumeSubHeadingListStart}{\begin{itemize}[leftmargin=0.15in, label={}]}
\newcommand{\resumeSubHeadingListEnd}{\end{itemize}}
\newcommand{\resumeItemListStart}{\begin{itemize}}
\newcommand{\resumeItemListEnd}{\end{itemize}\vspace{-10pt}}
\begin{document}
%-------------------------------------------

%----------HEADING-----------------
\begin{center}
    {\LARGE \textbf{ANBARASAN AYYAVU}}\\[4pt]
    {\large \textbf{AI Engineer}}\\[4pt]
    \small
    \faPhone\ +91-9894988646 \quad | \quad
    \href{mailto:anbarasan5612@gmail.com}{\faEnvelope\ anbarasan5612@gmail.com} \quad | \quad
    \href{https://www.linkedin.com/in/anbarasanayyavu}{\faLinkedin\ LinkedIn} \quad | \quad
    \href{https://github.com/anbarasanhere}{\faGithub\ GitHub} \quad | \quad
    \href{https://anbarasan.vercel.app/}{\faGlobe\ Portfolio}
\end{center}

\vspace{-5pt}

%-----------SUMMARY-----------------
\section{Summary}

AI Engineer and Data Scientist specializing in multi-agent system architectures, RAG and high performance data engineering. Proven track record in governing end-to-end project life cycles and executing unit testing and resolving 400+ critical production defects. Combines full-stack development with advanced business intelligence, engineering scalable Power BI ETL pipelines (DAX, Power Query) to transform complex enterprise system logic into real-time operational metrics.

%-----------SKILLS-----------------
\section{Technical Skills}

\textbf{Languages \& Frameworks:} Python, SQL, Pandas, NumPy, TensorFlow, Scikit-Learn, LangChain, LangGraph}

\textbf{Tools, DevOps \& Backend:} PowerBI, GitHub, Docker, Bash, FastAPI, ChromaDB, PostgreSQL

%-----------EXPERIENCE-----------------
\section{Experience}
\resumeSubheading
{HP}{}
{Software Engineering Analyst (Applied AI) } {Apr 2025 -- Present}

\resumeItemListStart

\item 
Managed end-to-end Knowledge Engineering (KE) workflows within the KBIDE framework—from project setup to production publishing—authoring SAP HANA (MS4) system rules, executing unit testing in the BB tool, resolving 400+ defects via JIRA/PST across QA validation cycles, and engineering Power BI dashboards (DAX, Power Query) for real-time operational tracking.
\item 
Deployed a RAG-based knowledge assistant for internal teams to refer process documentation with high answer accuracy—built on FastAPI, custom HTML/SSE UI, LangChain, ChromaDB, and OpenAI (Docker Compose)—covering document ingest, recursive chunking (700/100), `text-embedding-3-small` (1536-d) indexing of documents into Chroma (kbide-knowledge, 163 chunks), TOP-K similarity retrieval with score-threshold gating, 3-agent routing (Knowledge / Troubleshooting / Rules), and `gpt-4o-mini` streaming with source citations; hardened and tested LLM guardrails (API token auth, ~30 req/min rate limits, injection/topic filters, output sanitization, groundedness checks, audit logging); and evaluated document retrieval, agent routing, and safety via a 28-case golden set at 28/28 (100\%) plus guardrail unit tests.
\resumeItemListEnd

\resumeSubheading
{HCL - GUVI}{}
{Business Analytics Instructor - Freelance} {May 2025 -- Present}

\resumeItemListStart
\resumeItem{Responsibility}
{Mentored 200+ students to develop industry-level analytical skills using Advanced SQL, Power BI, Python, ML, Data Ethics,
Privacy, and Security in AI}
\resumeItemListEnd



%-----------EDUCATION-----------------
\section{Education}

\resumeSubheading
{Woolf University}{Malta}
{M.Sc. in Artificial Intelligence \& Machine Learning - (GPA 3.7/4.0)}{Apr 2024 -- Aug 2026}
\resumeItemListStart
\item
{Completed a \textbf{90 ECTS}, 18-month program comprising 2,250 hours, focused on \textbf{AI/ML \& Data Science}.}
\resumeItemListEnd

\resumeSubheading
{Arul Anandar College}{India}
{M.Sc. in Physics - (CGPA 7/10)}{Jun 2018 -- Jun 2020}
\resumeItemListStart
\item
{Studied Applied Electronics and Quantum Mechanics with hands-on experience in experimental physics.}
\resumeItemListEnd

%-----------PROJECTS-----------------

\section{Projects}
\resumeSubHeadingListStart
\resumeSubItem{Production-Aware AI Support Ticket Classifier \hspace{1pt}
\href{https://github.com/anbarasanhere/AI_Support_ticket_Classifier}{\faGithub}}
\resumeItemListStart
\item Engineered a 6-node \textbf{LangGraph} pipeline to classify and route raw tickets across 7 categories and 5 owner teams, exposed via a \textbf{FastAPI} REST service with \textbf{Pydantic} request/response contracts.
\item Implemented pre-LLM production safety including in-process \textbf{PII redaction} (emails, phones, credit cards) and a guard model for \textbf{prompt-injection detection} that routes untrusted inputs to human review.
\item Hardened LLM reliability using \textbf{JSON-mode} generation, business-rule validation, and \textbf{Tenacity} exponential backoff retries with deterministic fallbacks to guarantee zero API crashes under model or schema failure.
\item Integrated prompt versioning and \textbf{tiktoken}-based per-request token and cost tracking for \textbf{GPT-4o-mini}, providing real-time observability over classification quality and spend.
\resumeItemListEnd

\resumeSubItem{Hybrid Natural Language \& SQL AI Analytics Platform \hspace{1pt}
\href{https://github.com/anbarasanhere/AI_DATA_COPILOT}{\faGithub}}

\resumeItemListStart
\item Engineered a dual-mode analytics platform using \textbf{FastAPI} and \textbf{MySQL}, enabling both conversational querying and direct SQL execution through an interactive web UI without modifying underlying data.
\item Automated schema introspection via \textbf{information\_schema} to dynamically discover tables, column profiles, indexes, and sample data, persisting structural context as \textbf{JSON/Markdown} artifacts.
\item Implemented schema-aware graph retrieval that isolates primary entities and expands one-hop join maps, supplying minimal context to the LLM for grounded \textbf{SELECT} query generation.
\item Hardened execution security using \textbf{SQLGlot} AST parsing (restricting to single \textbf{SELECT/WITH} statements) alongside \textbf{READ-ONLY} MySQL sessions, execution timeouts, and bounded result limits.
\resumeItemListEnd



\resumeSubItem{Multi-Agent LLM Chat App with LLMOps on AWS ECS\hspace{2pt}
\href{[https://github.com/anbarasanhere/Multi-Agent-AI-Application-with-LLMOps-AWS-Deployment](https://github.com/anbarasanhere/Multi-Agent-AI-Application-with-LLMOps-AWS-Deployment)}{\faGithub}}

\resumeItemListStart
\item Developed a full-stack agentic platform using \textbf{FastAPI} and \textbf{Streamlit}, enabling dynamic model selection across \textbf{Groq} (\textbf{Llama 3.3 70B}) and \textbf{Tavily} web search tools via a RESTful API.
\item Implemented a \textbf{LangGraph ReAct agent} featuring tool gating, model validation, structured request schemas, and custom error handling across a decoupled, multi-layer architecture.
\item Containerized the dual-service application using \textbf{Docker} with multi-port routing, packaging it as a modular, installable Python project for local and cloud runs.
\item Designed an end-to-end \textbf{Jenkins CI/CD} pipeline integrating \textbf{SonarQube} code quality analysis, container scanning, image management via \textbf{Amazon ECR}, and automated rollout to \textbf{AWS ECS Fargate}.
\resumeItemListEnd

\resumeSubItem{Production RAG Pipeline \& AWS Cloud Infrastructure \hspace{1pt}
\href{https://github.com/anbarasanhere/Medical-RAG-Chatbot-with-LLMOps-AWS-Deployment}{\faGithub}}

\resumeItemListStart
\item Engineered an end-to-end medical Q\&A RAG pipeline using \textbf{LangChain}, \textbf{Hugging Face MiniLM}, and \textbf{FAISS}, processing PDF documentation through recursive chunking and vector similarity search.
\item Integrated \textbf{Groq Llama 3.1 8B} with context-grounded prompt engineering, ensuring answers remain strictly bounded to retrieved medical texts to prevent hallucinations.
\item Delivered a full-stack \textbf{Flask} web application featuring session history, robust logging, and structured exception handling for vector store and LLM failures.
\item Automated an end-to-end \textbf{Jenkins CI/CD} pipeline featuring \textbf{Trivy} security scanning (HIGH/CRITICAL enforcement), \textbf{Docker} containerization, image hosting on \textbf{AWS ECR}, and deployment to \textbf{AWS App Runner}.
\resumeItemListEnd

\resumeSubItem{E-Commerce Supply Chain & Delivery Optimization Analytics \hspace{2pt}
\href{YOUR_GITHUB_REPOSITORY_URL}{\faGithub}}
\resumeItemListStart
\item Performed end-to-end SQL analysis on an 8-table e-commerce dataset in  \textbf{Google BigQuery}, uncovering explosive order growth \textbf{(329 → 54,011 orders)} using time-series and window function queries.
\item Identified São Paulo as the primary market generating \textbf{\$5.2M in order revenue} (\textbf{64\% higher} than the second-ranked state), formulating data-backed recommendations to optimize regional resource allocation.
\item Diagnosed logistics and fulfillment bottlenecks using \textbf{TIMESTAMP\_DIFF()}, revealing a \textbf{3x disparity} in delivery lead times between top and remote states (8 days vs. 29 days) to mitigate supply chain risks.
\item Analyzed temporal purchasing trends and payment patterns across \textbf{100K+ transactions}, surfacing peak ordering hours and credit-card dominance to drive targeted staffing and promotional strategies.
\resumeItemListEnd

\resumeSubHeadingListEnd

%-----------CERTIFICATIONS-----------------
\section{Certifications}
\resumeSubHeadingListStart
\resumeSubItem{Google Advanced Data Analytics Professional Certificate}
{Completed hands-on projects involving Python, exploratory data analysis, regression models, and machine learning pipelines.}

\resumeSubItem{Generative AI Fundamentals -- Databricks}
{Gained core proficiencies in large language models, prompt engineering, and vector databases within the Databricks platform.}

\resumeSubItem{Data Science Internship -- Unified Mentor}
{Applied advanced data manipulation and predictive modeling techniques to solve real-world business analytics problems.}
\resumeSubHeadingListEnd

\end{document}
