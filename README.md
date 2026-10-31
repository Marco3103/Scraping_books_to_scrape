# 📚 Books to Scrape - Python Web Scraper

Uno script di **Web Scraping** sviluppato in Python per estrarre cataloghi di libri completi da [Books to Scrape](https://books.toscrape.com/). Il progetto raccoglie dati strutturati su 1.000 libri attraverso 50 pagine di catalogo, salvandoli in un DataFrame Pandas ed esportandoli in formato CSV.

---

## 🚀 Panoramica del progetto
Questo progetto è stato realizzato per dimostrare competenze pratiche nell'estrazione di dati da pagine web dinamiche e statiche, combinando la velocità di `requests`/`BeautifulSoup` con la flessibilità di `Selenium` per la gestione del DOM e l'automazione del browser.

### 📊 Dati estratti
Per ciascun libro nel catalogo vengono raccolti i seguenti campi:
* **Titolo**: nome completo del libro
* **Valutazione in stelle**: conversione della classe CSS in un valore numerico da 1 a 5
* **Prezzo**: prezzo di vendita in sterline (£)
* **Disponibilità**: stato attuale dell'inventario (es. *In stock*).

---

## 🛠️ Tecnologie e librerie utilizzate
* **Python**
* **Selenium WebDriver**: per l'interazione con il browser e la gestione degli elementi dinamici in modalità *headless*
* **BeautifulSoup (bs4)** & **Requests**: per il parsing HTML e la gestione delle richieste HTTP
* **Pandas**: per la manipolazione, strutturazione e pulizia dei dati raccolti
* **Chromedriver Autoinstaller**: per configurare automaticamente il driver di Chrome compatibile.

---

## ⚙️ Funzionalità e best practices
* **Headless mode**: esecuzione del browser in background senza interfaccia grafica, ottimizzando le risorse di sistema
* **Explicit waits (`WebDriverWait`)**: sincronizzazione intelligente per attendere il caricamento effettivo degli elementi nel DOM prima di procedere all'estrazione
* **Robusta gestione degli errori (`try-except`)**: intercettazione di anomalie per singolo elemento o pagina, garantendo che lo script non si interrompa a metà dell'esecuzione
* **Web etiquette (polite scraping)**: inserimento di pause controllate (`sleep`) tra una richiesta e l'altra per non sovraccaricare il server target.

---

## 💡 Come Visualizzare il Progetto

Puoi esaminare il codice direttamente visualizzando il file .ipynb su GitHub oppure aprirlo tramite  Jupyter Notebook per testare l'interattività e l'esecuzione delle celle.