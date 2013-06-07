Description
----
  "VersoDeRapport" est un document qui permet de générer le verso du rapport de l'ISI,
  l'Institut Supérieur d'Informatique de l'Université Tunis El Manar, Ariana, Tunisie.

  La mise en page a été adapté en LaTeX par :
  M. Med Ali Mortadha DAHMANI, ISI 2013.

Installation
----
1. Modifier le fichier .tex (encodage UTF-8) afin de créer le verso du rapport.
2. Sur Windows utiliser TeXnicCenter ou TexMaker (testé et approuvé)

Utilisation/Exemple
----
```
\documentclass[11pt,a4paper]{report}
\usepackage[top=20mm,bottom=20mm,left=20mm,right=20mm]{geometry}
\usepackage[utf8]{inputenc}
\usepackage{arabtex}
\usepackage[LFE,LAE]{fontenc}
\usepackage[arabic]{babel}
\usepackage{pslatex}

\begin{document}
\renewcommand{\thepage}{}

\hspace*{-5mm}\textbf{\Huge الملخّص}\\\\ 
هذا التقرير يعرض مراحل تصميم و إنجاز مشروع ختم الدروس بعنوان: ..
\\
بعد ...
\\\\
{الكلمات المفاتيح: الهاتف المحمول، النظم المحمولة، ...}
%
\\

\vspace*{3cm}

\textLR{\Huge \textbf{Résumé}\\\\
\normalsize
Ce mémoire décrit les étapes de conception et de réalisation du projet de fin d'études intitulé : ...\\
Après ...\\}

\textLR{\textbf{Mots clés}: Téléphone Mobile, Système, Embarqué, ...
\\
}
\\

\vspace*{3cm}

\textLR{\Huge \textbf{Abstract}\\\\
\normalsize
This paper describes the steps of designing and achieving the project entitled : ...\\
After ...\\}

\textLR{\textbf{Keywords}: Mobile Phone, System, Embedded, ...\\
\\
}

\vspace*{3cm}

\textLR{\Large \textbf{Intitule et adresse complète de l'entreprise}\\\\
\normalsize
\textbf{Entreprise}: \dotfill\\
\textbf{Adresse}: \dotfill\\
\textbf{Tél.}: \dotfill\\ 
\textbf{Fax}: \dotfill\\  
\textbf{Email}: \dotfill\\ 
\\}
\end{document}
```
