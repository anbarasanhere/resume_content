%-------------------------
% Resume in LaTeX - Strict Single-Page Layout
%------------------------

\documentclass[a4paper,10pt]{article}
\usepackage[a4paper, left=0.4in, right=0.4in, top=0.4in, bottom=0.4in]{geometry}
\usepackage{latexsym}
\usepackage{titlesec}
\usepackage{marvosym}
\usepackage[usenames,dvipsnames]{color}
\usepackage{verbatim}
\usepackage{enumitem}
\usepackage[pdftex]{hyperref}
\usepackage{fontawesome5}

% Remove headers and footers to reclaim vertical space
\pagestyle{empty}
\urlstyle{same}
\raggedbottom
\raggedright
\setlength{\tabcolsep}{0in}
\setlength{\parskip}{0pt}

% Section Formatting & Distinct Spacing Between Sections
\titleformat{\section}{
  \vspace{-2pt}\scshape\raggedright\large
}{}{0em}{}[\color{black}\titlerule \vspace{1pt}]

\titlespacing*{\section}{0pt}{5pt}{3pt}

% Custom Commands
\newcommand{\resumeItem}[2]{
  \item\small{
    \textbf{#1}{: #2}
  }
}

\newcommand{\resumeSubheading}[4]{
  \item
    \begin{tabular*}{0.99\textwidth}{l@{\extracolsep{\fill}}r}
      \textbf{#1} & #2 \\
      \textit{\small#3} & \textit{\small #4} \\
    \end{tabular*}\vspace{-2pt}
}

\newcommand{\resumeSubItem}[1]{\item\small{#1}\vspace{-1pt}}

\renewcommand{\labelitemii}{$\circ$}

% Macros for left-most alignment and controlled spacing
\newcommand{\resumeSubHeadingListStart}{\begin{itemize}[leftmargin=0pt, label={}, noitemsep, topsep=0pt, parsep=0pt]}
\newcommand{\resumeSubHeadingListEnd}{\end{itemize}\vspace{0pt}}
\newcommand{\resumeItemListStart}{\begin{itemize}[leftmargin=10pt, topsep=1pt, parsep=0pt, itemsep=1.5pt]}
\newcommand{\resumeItemListEnd}{\end{itemize}\vspace{1pt}}

\begin{document}

%----------HEADING-----------------
\begin{center}
    {\LARGE \textbf{ANBARASAN AYYAVU}}\\[2pt]
    {\large \textbf{Data Scientist $|$ AI Engineer}}\\[2pt]
    \small
    \faPhone\ +91-9894988646 \quad | \quad
    \href{mailto:anbarasan5612@gmail.com}{\faEnvelope\ anbarasan5612@gmail.com} \quad | \quad
    \href{https://www.linkedin.com/in/anbarasanayyavu}{\faLinkedin\ LinkedIn} \quad | \quad
    \href{https://github.com/anbarasanhere}{\faGithub\ GitHub} \quad | \quad
    \href{https://anbarasan.vercel.app/}{\faGlobe\ Portfolio}
\end{center}

\vspace{-4pt}

%-----------SUMMARY-----------------
\section{Summary}
\small{Data Scientist and Applied AI Engineer with a Master’s in AI & Machine Learning, specializing in architecting end-to-end predictive models, enterprise data pipelines, and MLOps frameworks. Proficient in Python, SQL, Databricks, and Power BI with a strong track record of translating complex multi-source enterprise data into actionable business intelligence, real-time operational dashboards, and production-grade AI solutions.}

%-----------SKILLS-----------------
\section{Technical Skills}
\small{
  \textbf{Languages \& Frameworks:} Python, SQL, Pytorch, TensorFlow, Scikit-Learn, LangChain, LangGraph, AI Frameworks \\[2pt]
  \textbf{Tools, DevOps \& Backend:} FastAPI, GenAI, Agentic AI, MLOps, LLMs, GitHub, Docker, Bash
}

%-----------EXPERIENCE-----------------
\section{Experience}
\begin{itemize}[leftmargin=0pt, label={}, noitemsep, topsep=0pt]
  \resumeSubheading
    {HP}{}
    {Software Engineer (Applied AI)}{Apr 2025 -- Present}
    \begin{itemize}[leftmargin=10pt, topsep=1.5pt, parsep=0pt, itemsep=1.5pt]
      \item \textbf{LLM \& RAG Systems Engineering:} Engineered an end-to-end internal RAG assistant using \textbf{FastAPI}, \textbf{LangChain}, \textbf{ChromaDB}, and \textbf{OpenAI}, featuring recursive chunking, \textbf{3-agent routing}, top-k retrieval with score gating, and streaming citations.
      \item \textbf{Production Guardrails \& Reliability:} Hardened API security via authentication, rate limiting, prompt-injection defense, and audit logging; validated routing and safety pipelines using a \textbf{28-case golden evaluation set} and unit testing.
      \item \textbf{Knowledge Engineering \& System Ops:} Managed production rule authoring workflows, resolved \textbf{400+} defects across QA validation cycles, and engineered real-time \textbf{Power BI} operational tracking dashboards.
    \end{itemize}

  \vspace{2pt}

  \resumeSubheading
    {HCL -- GUVI}{}
    {Data Science - Gen AI Instructor (Freelance)}{May 2025 -- Present}
    \begin{itemize}[leftmargin=10pt, topsep=1.5pt, parsep=0pt, itemsep=1.5pt]
      \item \textbf{Mentorship \& Instruction:} Upskilled working professionals and cross-functional teams in developing industry-ready analytical capabilities using Advanced SQL, Power BI, Python, Machine Learning, NLP, CV, GenAI and Data Ethics.
    \end{itemize}

  \vspace{2pt}

  \resumeSubheading
    {SAN}{}
    {Head of Physics}{May 2022 -- Apr 2024}
    \begin{itemize}[leftmargin=10pt, topsep=1.5pt, parsep=0pt, itemsep=1.5pt]
      \item \textbf{Physics \& Robotics:} Designed Arduino setups for Simple Harmonic Motion, built self-driving obstacle-avoidance robots, and integrated MATLAB for pulse frequency analysis.
    \end{itemize}
\end{itemize}

%-----------EDUCATION-----------------
\section{Education}
\begin{itemize}[leftmargin=0pt, label={}, noitemsep, topsep=0pt]
  \resumeSubheading
    {Woolf University}{Malta}
    {M.Sc. in Artificial Intelligence \& Machine Learning -- (GPA: 3.7/4.0)}{Apr 2024 -- Aug 2026}
  \resumeSubheading
    {Arul Anandar College}{India}
    {M.Sc. in Physics -- (CGPA: 7.0/10)}{Jun 2018 -- Jun 2020}
\end{itemize}

%-----------PROJECTS-----------------
\section{Projects}
\resumeSubHeadingListStart

\resumeSubItem{\textbf{Enterprise AI Support Ticket Classifier \& Router} $|$ \emph{Python, LangGraph, FastAPI, Pydantic, Tenacity} \hspace{1pt}
\href{https://github.com/anbarasanhere/support-ticket-classifier}{\faGithub}}
\resumeItemListStart
\item \textbf{Problem \& Solution:} Engineered a production-ready, 6-node \textbf{LangGraph} pipeline exposed via a \textbf{FastAPI} REST service with \textbf{Pydantic} contracts to automatically classify raw tickets across 7 categories and route them to 5 owner teams, eliminating manual triage bottlenecks.
\item \textbf{Reliability \& Security:} Implemented pre-LLM production safety using in-process \textbf{PII redaction}, a \textbf{prompt-injection guard model}, \textbf{JSON-mode} generation, and \textbf{Tenacity} exponential backoff retries with deterministic fallbacks for zero API crashes.
\item \textbf{Performance \& LLMOps:} Integrated prompt versioning alongside \textbf{tiktoken}-based per-request token and cost tracking for \textbf{GPT-4o-mini}, delivering real-time observability over classification quality, latency, and spend.
\resumeItemListEnd

\resumeSubItem{\textbf{Natural Language to SQL Data Copilot} $|$ \emph{Python, FastAPI, MySQL, SQLGlot, OpenAI, SQLAlchemy} \hspace{1pt}
\href{https://github.com/anbarasanhere/AI_DATA_COPILOT}{\faGithub}}
\resumeItemListStart
\item \textbf{Problem \& Solution:} Engineered a dual-mode analytics platform using \textbf{Python}, \textbf{FastAPI}, and \textbf{MySQL} to enable both direct SQL execution and grounded conversational querying while preserving underlying data.
\item \textbf{Operations:} Automated schema introspection via \textbf{information\_schema} to persist structural context, building graph retrieval that expands one-hop join maps for minimal LLM context window usage.
\item \textbf{Performance \& Security:} Guaranteed 100\% mutation prevention using \textbf{SQLGlot} AST parsing (restricting to single \textbf{SELECT/WITH} statements), \textbf{READ-ONLY} MySQL sessions, execution timeouts, and bounded result limits.
\resumeItemListEnd

\resumeSubItem{\textbf{Multi-Agent AI Application with LLMOps \& AWS Deployment} $|$ \emph{Python, LangGraph, FastAPI, Docker, AWS, Jenkins} \hspace{1pt}
\href{https://github.com/anbarasanhere/Multi-Agent-AI-Application-with-LLMOps-AWS-Deployment}{\faGithub}}

\resumeItemListStart
\item \textbf{Architecture \& Agentic Systems:} Developed a full-stack agentic platform using \textbf{FastAPI} and \textbf{Streamlit}, implementing a \textbf{LangGraph ReAct agent} featuring tool gating, model validation, and dynamic model selection across \textbf{Groq} and \textbf{Tavily}.
\item \textbf{Containerization \& Modular Engineering:} Containerized the dual-service application using \textbf{Docker} with multi-port routing, packaging structured request schemas and custom error handling into a modular Python project for local and cloud environments.
\item \textbf{LLMOps \& Automated Deployment:} Designed an end-to-end \textbf{Jenkins CI/CD} pipeline integrating \textbf{SonarQube} code quality analysis, container security scanning, image management via \textbf{Amazon ECR}, automated rollout to \textbf{AWS ECS Fargate}.
\resumeItemListEnd
\resumeSubHeadingListEnd

%-----------CERTIFICATIONS-----------------
\section{Certifications}
\begin{itemize}[leftmargin=10pt, topsep=1pt, parsep=0pt, itemsep=1pt]
  \item \textbf{Google Advanced Data Analytics Professional Certificate:} Hands-on projects involving Python, exploratory data analysis, regression models, and ML pipelines.
  \item \textbf{Generative AI Fundamentals -- Databricks:} Proficiencies in large language models, prompt engineering, and vector databases.
\end{itemize}

\end{document}
