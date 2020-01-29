# Unibo Tesi

[![Build Status](https://travis-ci.com/NiccoMlt/Unibo-Tesi.svg?branch=master)](https://travis-ci.com/NiccoMlt/Unibo-Tesi)
[![Commitizen friendly](https://img.shields.io/badge/commitizen-friendly-brightgreen.svg)](http://commitizen.github.io/cz-cli/)
[![made-with-latex](https://img.shields.io/badge/Made%20with-LaTeX-1f425f.svg)](https://www.latex-project.org/)
[![made-for-VSCode](https://img.shields.io/badge/Made%20for-VSCode-1f425f.svg)](https://code.visualstudio.com/)
[![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)

Template LaTeX per una tesi per l'Università di Bologna, Dipartimento di Informatica - Scienza e Ingegneria.

## Tutorial

Utilizzare il bottone <kbd>Use this template</kbd> per generare un nuovo repository per realizzare la propria tesi di laurea.

[![Use this template explaination](https://help.github.com/assets/images/help/repository/use-this-template-button.png)](https://help.github.com/en/articles/creating-a-repository-from-a-template)

Per l'utilizzo, si consiglia di utilizzare una versione recente di TeXLive (2018+), di MikTeX o di MacTeX (non testato) e di avere installato un Java Runtime Environment con versione compresa tra 5 e 10 (testato OpenJDK 8).

Inoltre, si consiglia di installare Python 3.x e il pacchetto `pygments` per permettere l'evidenziazione del codice.

Vedere la sezione [Dettagli tecnici](#dettagli-tecnici) per ulteriori dettagli.

## Consigli

### Linguaggio

- Evitare sempre commenti non oggettivi/superficiali/informali (o sono supportati da citazioni o non si mettono).
  Ad esempio: _banale_, _semplice_, _facile_, _difficile_, _molto_, _troppo_, _poco_, _impossibile_.
- **Concisione**: Non scrivere frasi più lunghe di _due_ righe.
- Evitare l'abuso di **grassetto** e _corsivo_.
- il _corsivo_ è per l'enfasi, di conseguenza si consiglia di utilizzarlo per evidenziare una parola.
  Usare `\emph{}` anziché `\textit{}`:
  `\emph{}` capisce da solo come mettere in evidenza in modo diverso in casi diversi (non sempre in corsivo).
- il **grassetto** è per una maggiore enfasi e, nella maggior parte dei casi, dovrebbe essere evitato.
  Nel caso si intenda utilizzarlo, usare `\strong{}` anziché `\textbf{}`.

### Inglesismi

- Se le tesi è in italiano è bene scrivere in italiano e limitare l'uso dell'inglese il più possibile.
- Usa un termine inglese se questo si ripete ma spiegalo una sola volta.
- Un acronimo in inglese rimane in inglese.
- La prima volta in assoluto che il termine compare scrivilo in corsivo.

### Capitoli, Sezioni e Paragrafi

- La classe è di tipo libro e, come tale, ha una gerarchia di questo tipo:
  1. `\frontmatter`, `\mainmatter` e `\backmatter` (per distinguere le numerazioni)
  2. `\chapter`
  3. `\section`
  4. `\subsection`
  5. `\subsubsection`
- Usare i riferimenti di Latex e le `label` per fare riferimento a capitoli/sezioni/sottosezioni/immagini:
  - `\Cref{}` capisce automaticamente che tipo di cosa si sta riferendo, aggiungendola prima del numero.
  - `\Vref{}` aggiunge anche la pagina oltre al tipo.
  - <ins>**Non** usare il vecchio `\ref{}`</ins> specificando a mano cosa è cosa.
  - Usare `Cref` e `Vref` e non le varianti minuscole `cref` e `vref`.
  - Quando si descrive un argomento è bene averlo già introdotto: se non indispensabili, evitare dunque le _forword reference_ (riferimento a capitoli/sezioni/sottosezioni che appaiono dopo essere referenziati).
- Non creare sezioni con singola sottosezione, o capitoli con un singola sezione.
- C'è differenza tra `.` e `. a capo`: `. a capo` si usa per cambiare discorso.
- Evitare di disperdere le informazioni: _definizione_, _dettagli_ e _implicazioni_ stanno nello stesso paragrafo.

### Citazioni

- Non citare Wikipedia, ma sfruttarla insieme a Google Scholar per trovare le citazioni a paper/libri.
- Non copiare testi troppo lunghi, è meglio riassumerli ed elaborarli.
- Non copiare traduzioni troppo lunghe, è meglio riassumerle ed elaborarle.
- Esplicita la parte di testo copiata inserendola tra virgolette e aggiungi la citazione finale.
  - il pacchetto `csquotes` offre alcuni comandi utili per virgolettare il testo.
  - usa `\cite{}` per citare il riferimento dalla bibliografia e usa `~` invece dello spazio per mantenerla sulla stessa riga del testo citato.

### Figure

- Se una figura è copiata/rielaborata indica la sorgente.
- Utilizzare figure in formato vettoriale: PostScript (`.eps`), PDF, SVG.
- in caso di screenshot, attenzione alle dimensioni (in MB) della figura.

### Punteggiatura, elenchi e coerenza

- No punti nei titoli.
- Non `E'` ma `È` (`È` = <kbd>Alt</kbd> + 0200 su Windows, tastiera italiana).
- Elenchi puntati iniziano con Maiuscola, finiscono con `;` o con `.` (l'importante è usare la stessa convenzione).
  - Di solito si usa `;` per terminare frasi di senso non compiuto, e `.` per terminare frasi di senso compiuto.
- No `...`, sì "`etc.`".

## [Requisiti](https://corsi.unibo.it/magistrale/IngegneriaScienzeInformatiche/volume-pdf-e-deposito-online-dellelaborato) e [Norme redazionali](https://corsi.unibo.it/magistrale/IngegneriaScienzeInformatiche/redazione-tesi-voto-finale) della tesi

- È vietato riprodurre il logo dell'Ateneo di Bologna su qualunque parte dell'elaborato;
- il file non dovrà superare i 30Mb;
- pagine di 32-35 righe, ciascuna di 65-70 caratteri di tipo prestabilito (Times New Roman, Arial, Courier o Helvetica);
- lunghezza dell’elaborato compresa fra le 50.000 e le 100.000 battute (spazi inclusi);
- corpo del testo di 12 o 13 punti (le note vanno in corpo 10);
- margini destro-sinistro e superiore-inferiore di 2,5 cm;
- interlinea 1,5 cm;
- frontespizio conforme al [fac-simile](https://corsi.unibo.it/magistrale/IngegneriaScienzeInformatiche/volume-pdf-e-deposito-online-dellelaborato/frontespiziolmisi.pdf/@@download/file/FrontespizioLMISI.pdf);
- figure e tavole in formato UNI (A4 e A3);
- il file deve essere nominato nel modo: `cognome_nome_tesi`;
- formato PDF.

## Dettagli tecnici

Il template è pensato per essere usato con il motore **LuaLaTeX** e non il "tradizionale" pdfLaTeX che ho già utilizzato in passato anche nella [mia tesi di laurea triennale](https://github.com/NiccoMlt/alchemist-thesis).

Inoltre, per semplificare il processo di sviluppo del documento, si intende supportare [**arara**](https://github.com/cereda/arara) come _build tool_ e **VisualStudio Code** come _ambiente di lavoro_, grazie all'ausilio del plugin [**LaTeX Workshop**](https://marketplace.visualstudio.com/items?itemName=James-Yu.latex-workshop).

Il template utilizza la classe [`scrbook`](https://www.ctan.org/pkg/scrbook) (alternativa della collezione [KOMA-script](https://www.ctan.org/pkg/koma-script) della classe `book`) e definisce una dimensione del testo di 12pt, con margini identici di 2,5cm e interlinea con scartamento 1,5.

Il font utilizzato è il _Latin Modern_ OpenType in tutte le varianti.

Il PDF generato è conforme allo standard PDF/A-1b.

La bibliografia è gestita tramite backend [`biber`](https://ctan.org/pkg/biber) e pacchetto [`biblatex`](https://www.ctan.org/pkg/biblatex);
il database [`biblio.bib`](./biblio.bib) può essere editato a mano o con strumenti come [JabRef](http://www.jabref.org/).

Lo stile scelto per la biblografia è quello [_IEEE_](https://ctan.org/pkg/biblatex-ieee).

## Riferimenti

Per la realizzazione del template sono state molto utili, oltre a questi ultimi anni di utilizzo di LaTeX per la stesura di numerosi documenti, le guide fornite dal [GuIT](https://www.guitex.org/home/it/doc).

In particolare, segnalo:

- Per approfondire LaTeX in generale:
    - [L’arte di scrivere con LaTeX](http://www.lorenzopantieri.net/LaTeX_files/ArteLaTeX.pdf), di Lorenzo Pantieri e Tommaso Gordini;
    - [LaTeX per l’impaziente](http://www.lorenzopantieri.net/LaTeX_files/LaTeXimpaziente.pdf), di Lorenzo Pantieri;
    - [Breve guida ai pacchetti di uso più comune](http://profs.sci.univr.it/~gregorio/breveguida.pdf), di Enrico Gregorio;
    - [LaTeXpedia](http://www.lorenzopantieri.net/LaTeX_files/LaTeXpedia.pdf), di Lorenzo Pantieri.
- Per approfondire LuaLaTeX:
    - [Introduzione a XeLaTeX](http://profs.sci.univr.it/~gregorio/introxelatex.pdf), di Enrico Gregorio;
    - [L’arte di scrivere in diverse lingue con XeLaTeX](http://www.guitex.org/home/images/doc/ArteLingue.pdf), di Claudio Beccari;
    - [Creare file archiviabili con pdfLaTeX e LuaLaTeX](http://www.guitex.org/home/images/doc/GuideGuIT/filearchiviabili.pdf), di Claudio Beccari.
    - [lualatex-doc](http://ctan.mirror.garr.it/mirrors/CTAN/info/luatex/lualatex-doc/lualatex-doc.pdf)
- Per approfondire la gestione di font e tipografia:
    - [Tipocomporre in italiano](http://www.guitex.org/home/images/doc/GuideGuIT/ComporreItaliano.pdf), di Claudio Beccari;
    - [Font e tipografia](http://www.guitex.org/home/images/doc/GuideGuIT/guidafont.pdf), di Claudio Beccari.
- Per approfondire arara:
    - [Introduzione a arara](http://profs.sci.univr.it/~gregorio/introarara.pdf), di Enrico Gregorio;
    - [arara package documentation](http://mirrors.ctan.org/support/arara/doc/arara-manual.pdf) per la versione 4.x.x del pacchetto.
- Per approfondire cose utili per una tesi:
    - [Scrivere la tesi di laurea in LaTeX](http://www.guitex.org/home/images/doc/GuideGuIT/IntroTesi.pdf), di Agostino De Marco;
    - [La bibliografia in biblatex e i programmi di gestione dei record](http://www.guitex.org/home/images/doc/GuideGuIT/bibliografia.pdf), di Filippo Vomiero;
    - [BibLaTeX package documentation (English)](http://ctan.mirror.garr.it/mirrors/CTAN/macros/latex/contrib/biblatex/doc/biblatex.pdf);
    - [TOPtesi Class documentation (Italian)](http://ctan.mirror.garr.it/mirrors/CTAN/macros/latex/contrib/toptesi/toptesi-it.pdf), di Claudio Beccari;
    - [frontespizio package documentation (Italian)](http://ctan.mirror.garr.it/mirrors/CTAN/macros/latex/contrib/frontespizio/frontespizio.pdf).

## Licenza

Il codice del documento è stato personalmente realizzato dal sottoscritto Niccolò Maltoni interpretando le norme relazionali del Dipartimento di Informatica, Scienza e Ingegneria dell'Università di Bologna pubblicate sul sito e cercando di allinearle agli standard tipografici italiani appresi con la lettura parziale del materiale linkato sopra.

Il codice realizzato è inteso come un prodotto personale indipendente dall'Università di Bologna;
per quanto io intenda utilizzare questo documento per la mia tesi di laurea magistrale, in nessun modo mi ritengo responsabile della produzione di documenti non validi a un utilizzo ufficiale di qualsiasi tipo tramite l'impiego di questo template.

Il codice è fornito sotto licenza [Apache License, Version 2.0](https://opensource.org/licenses/Apache-2.0) in accordo al file [`LICENSE`](./LICENSE) incluso in questo repository.
