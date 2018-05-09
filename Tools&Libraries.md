# Tools



## Text Summarizer

- Open Source auf github (https://github.com/karimo94/Text-Summarizer)
- Simpler Ablauf:
  - nimmt Wörter mit Anzahl in Map
  - entfernt häufige wie "and" oder "because"
  - sortiert nach Menge
  - teilt Text in Sätze welche nach Häufigkeit der Wörter aufgenommen werden
- Implementation dort ist fehlerhaft, vom Prinzip her aber einfach selbst zu schreiben



## TextTeaser

- Python, MIT Lizenz (d.H. dürfen wir nutzen) https://github.com/IndigoResearch/textteaser
- Ablauf komplexer, aber präziser
  - Keyword Liste
  - Sortiert Sätze mit gewichtetem Ansatz
  - vergleicht mit Titel
  - bezieht Position im Text mit ein
  - bezieht Länge des Satzes mit ein



## autosummarizer.com

- Webbasiert: http://autosummarizer.com
- Web basiert
- aktuell wenig hilfreich, weil Quellcode nicht einsehbar



## SMMRY

- Webbasiert: https://smmry.com
- Kein einsehbarer Quellcode
- Viele Optionen:
  - Anzahl der Sätze
  - Fragen, Ausrufe, Zitate vermeiden
  - Eigene Keywords angeben
  - Heatmap um wichtige Sätze hervorzuheben



# Libraries

## Open-Text-Summarizer

- Library für z.B. https://www.splitbrain.org
- Visible Source: https://github.com/neopunisher/Open-Text-Summarizer
- GPL Lizenz (d.H. wir dürfen es nutzen solange wir angeben wo es herkommt)
- Native Unterstützung für diverse Sprachen
- Shell-basiert, geschrieben in C (daher, leider nicht so leicht zu lesen)
- Keyword-Ansatz, aber mit "Stemming" Funktion, d.H, Wortstämme erkennen und diese bei Vergleichen mit einbeziehen



##  SUMY

- Python
- Visible Source: https://github.com/miso-belica/sumy
- Apache Lizenz (für uns nutzbar)
- Bietet verschiedene Zusammenfassungsverfahren
- Kann HTML verarbeiten



### NLTK

- Natural Language Toolkit, Python Bibliothek zum Verabeiten von Sprache

- www.ntlk.org und https://github.com/nltk/nltk

- Apache Lizenz (für uns nutzbar)

- Fasst selbst nicht zusammen, kann aber Keyword-Listen erstellen und Stopwörter filtern

  