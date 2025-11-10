# Systeminstruktionen

## Kontext

- Ich bin *Professor für Informatik und Industriesysteme* an der *Fakultät für Technik und angewandte Naturwissenschaften* der *Fachhochschule Oberösterreich* am *Campus Wels*.
- Ich unterrichte im **Englisch**-sprachigen Bachelor-Studiengang "Innovation, Product & Engineering Management", in dem die Studierenden zu Produktmanagern ausgebildet werden.
- Dieses Repostitory enthält meine Unterlagen für den Kurs *Programmieren mit Python*, in dem die Studierenden die Grundlagen der Programmierung erlernen.

## Lernziele

- Quelltext lesen und verstehen.
- Einfache Quelltexte selber schreiben.
- Fehleranalyse und -behebung mittels Debugger.
- Aufbau und Funktionsweise von Quelltexten dokumentieren.

## Kursorganisation

- 10 Präsenztermine
- Dauer der Präsenztermine ist 2,5 Stunden
- Eigener Foliensatz für jeden Präsenztermin
- Hausübungen nach jedem Präsenztermin
- Prüfung zu Beginn jedes folgenden Präsenztermins
- Die Art der Prüfung ist ein Multiple-Choice-Test
- Die Dauer der Prüfung ist 20 Minuten
- Für die Prüfung sind keine Hilfsmittel zugelassen

## Präsentationstechnik

Die Folien für die einzelnen Termine sind mit Latex Beamer gemacht. Der Latex-Quelltext der Folien ist wie folgt strukturiert:

```latex
\documentclass[aspectratio=169,8pt]{beamer}

% Laden des eigenen Beamer-Themes
\newcommand{\basepath}{../../../latex-beamer-theme-fhooe/sources}
\usepackage{\basepath}

\title{Programmieren mit Python}
\subtitle{Termin X: ...}
\author{Dr. Georg Hackenberg}
\institute{FH Oberösterreich}
\date{\today}

\begin{document}

\begin{frame}
    \titlepage
\end{frame}

\section{Titel des Abschnitts}

\subsection{Titel des Unerabschnitts}

% Vorlage für Folie mit einer Spalte
\frameOneColumn{}{Titel der Folie}{c}{
    Inhalt der Folie
}

% Vorlage für Folie mit zwei Spalten
\frameTwoColumn{}{Titel der Folie}{c}{
    Inhalt der ersten Spalte
}{
    Inhalt der zweiten Spalte
}

% Vorlage für Folie mit drei Spalten
\frameOneColumn{}{Titel der Folie}{c}{
    Inhalt der ersten Spalte
}{
    Inhalt der zweiten Spalte
}{
    Inhalt der dritten Spalte
}

\end{document}
```

## Ordnerstruktur

- Der Ordner `./Unterlagen` enthält die Unterlagen für die einzelnen Termine
- Der Ordner `./Unterlagen/Termin_XX` enthält den Foliensatz für Termin `XX`
- Die Datei `./Unterlagen/Termin_XX/Folien.tex` enthält den Latex-Quelltext für den Foliensatz von Termin `XX`
- Der Ordner `./Unterlagen/Termin_XX/Übungsblätter` enthält die Übungsblätter für Termin `XX`
- Die Datei `./Unterlagen/Termin_XX/Übungsblätter/Übungsblatt_YY.tex` enthält das Übungsblatt `YY` für Termin `XX`
- Der Ordner `./Unterlagen/Termin_XX/Prüfungsangaben` enthält die Prüfungsangaben für Termin `XX`
- Die Datei `./Unterlagen/Termin_XX/Prüfungsangaben/Prüfungsangabe_YY.tex` enthält die Prüfungsangabe `YY` für Termin `XX`