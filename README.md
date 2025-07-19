\documentclass{article}
\usepackage[a4paper,margin=1in]{geometry}
\usepackage{hyperref}
\usepackage{enumitem}

\begin{document}

\begin{center}
    \LARGE \textbf{Multimodal RAG System for\\ Scientific Question Answering}
\end{center}

\section*{Overview}
A system to answer complex scientific questions by retrieving and reasoning over \textbf{text, tables, and images} in research papers. Built with \textbf{LLaMA3}, \textbf{LLaVA}, \textbf{LangChain}, and \textbf{ChromaDB}.

\section*{Features}
\begin{itemize}[noitemsep,topsep=0pt]
    \item Parse and embed multimodal content (text, tables, images)
    \item Store/retrieve embeddings via ChromaDB
    \item Retrieval-augmented answers using LLaMA3 and LLaVA
    \item Modular pipeline powered by LangChain
\end{itemize}

\section*{Quick Start}
\begin{enumerate}[noitemsep,topsep=0pt]
    \item \textbf{Clone:} \texttt{git clone https://github.com/your-repo.git}
    \item \textbf{Install:} \texttt{pip install -r requirements.txt}
    \item \textbf{Prepare models:} Download LLaMA3 and LLaVA weights
    \item \textbf{Index data:}\\
          \texttt{python index\_documents.py --input\_folder data/}
    \item \textbf{Ask a question:} \\
          \texttt{python ask.py --question "Your question here"}
\end{enumerate}

\section*{Project Layout}
\begin{verbatim}
data/        # Papers
modules/     # Parsing & embedding
index_documents.py
ask.py
\end{verbatim}

\section*{License}
MIT

\noindent
\textit{Acknowledgements: LLaMA3, LLaVA, LangChain, ChromaDB.}
\vspace{1em}

\noindent
\textbf{Note:} Ensure compliance with model/data licenses.

\end{document}
