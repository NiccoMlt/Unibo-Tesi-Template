# Unibo Tesi

[![Commitizen friendly](https://img.shields.io/badge/commitizen-friendly-brightgreen.svg)](http://commitizen.github.io/cz-cli/)

Template LaTeX per una tesi Unibo

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
- Per approfondire la gestione dei font:
    - [Tipocomporre in italiano](http://www.guitex.org/home/images/doc/GuideGuIT/ComporreItaliano.pdf), di Claudio Beccari;
    - [Font e tipografia](http://www.guitex.org/home/images/doc/GuideGuIT/guidafont.pdf), di Claudio Beccari.
- Per approfondire arara:
    - [Introduzione a arara](http://profs.sci.univr.it/~gregorio/introarara.pdf), di Enrico Gregorio;
    - [arara package documentation](http://mirrors.ctan.org/support/arara/doc/arara-manual.pdf) per la versione 4.x.x del pacchetto.
- Per approfondire cose utili per una tesi:
    - [Scrivere la tesi di laurea in LaTeX](http://www.guitex.org/home/images/doc/GuideGuIT/IntroTesi.pdf), di Agostino De Marco;
    - [La bibliografia in biblatex e i programmi di gestione dei record](http://www.guitex.org/home/images/doc/GuideGuIT/bibliografia.pdf), di Filippo Vomiero;
    - [TOPtesi Class documentation (Italian)](http://ctan.mirror.garr.it/mirrors/CTAN/macros/latex/contrib/toptesi/toptesi-it.pdf), di Claudio Beccari.
