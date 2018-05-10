##Code

1. Pakete Importieren
   - from gensim.summarization.summarizer import summarize
   - from gensim.summarization import keywords
   - from bs4 import BeautifulSoup
   - from urllib.request import urlopen
2. Textdatei öffnen, Inhalt abspeichern
	- fname = "C:/Users/username/Desktop/file"
	- with open(fname, 'r') as myfile:
      text = myfile.read()
3. URL öffnen, Inhalt abspeichern
	- page = urlopen(url)
    - soup = BeautifulSoup(page, "lxml")
    - text = ' '.join(map(lambda p: p.text, soup.find_all('p')))
    - return soup.title.text, text
4. Ausgabe
	- print('Zusammenfassung:')
	- print(summarize(text, ratio=0.01))
	- print('\nSchluesselwoerter:')
	- print(keywords(text, ratio=0.01))
	- url = "https://de.wikipedia.org/wiki/Python_(Programmiersprache)"
	- text = get_only_text(url)
	- print('Zusammenfassung:')
	- print(summarize(str(text), ratio=0.01))
	- print('\nSchluesselwoerter:')
	- print(keywords(str(text), ratio=0.01))


##Beurteilung
- Nicht für jede Webseite gedacht( Wikipedia klappt   fast immer)
- Textdatei: Text muss lang genug sein, sonst keine   oder sehr kurze Zusammenfassung
- Das Programm ist viel zu langsam, wenn der Text    zu lang ist
- Zusammenfassung oft nicht gut



