uscki LaTeX Package
===========

LaTeX package welke USCKI-logo's als symbolen beschikbaar maakt voor de LaTeX-gebruiker.

Deze package is bedoeld voor leden van de Utrechtse Studievereniging van Cognitieve Kunstmatige Intelligentie: Incognito en maakt het mogelijk Logo's van de vereniging in LaTeX te gebruiken.

Deze package laadt logo's van de vereniging in, zodat deze met een simpel commando bruikbaar zijn.
Op het moment van schrijven zijn, bij weten van ondergetekende, alle versies van logo's van USCKI Incognito en van alle subcommissies die beschikbaar zijn verwerkt.

<h3>Gebruik</h3>
Voor het gebruik van deze package moet deze worden geïnstalleerd, of moeten de volgende bestanden in dezelfde map staan of moet de package worden:
  - ckilogos.ttf
  - ckilogos.tfm
 	- uscki.sty
  - jouw .TeX-bestand

Bij het aanroepen probeert deze package een declaratie toe te voegen aan het LaTeX mapbestand.
Als dit niet lukt, zal het lettertype niet bruikbaar zijn.

Package kan na de installatie worden aangeroepen met:
```Tex
\usepackage{uscki}
```

Lijst van commando's met bijbehorende logo's
```TeX
\cki        # CKI-letters in huisstijl
\AI         # CKI-letters in huisstijl, inclusief de punt op de i
\USCKI      # USCKI-logo
\ABCLogo    # ABC-logo
\Bata       # Bata-logo
\cafeCKI    # Café-CKI-logo
\DraeCKI    # DraeCKI-logo
\LoeCKI     # LoeCKI-logo
\SympoCKI   # Symposiumcommissielogo
```

<h3>Installatieinstructies</h3>
LaTeX maakt gebruik van tree structures om bestanden van de packages in te ordenen. Deze package maakt gebruik van die tree structure en zal alleen werken als die structuur wordt vastgehouden.

Maak een nieuwe map aan buiten de installatiedirectory van LaTeX, bijvoorbeeld _texmf_  in _Mijn Documenten_

Zorg dat de bestanden uit deze package op de volgende manier in de _texmf_-map komen:

    texmf
    |             
    |              
    |_______ Fonts
    |           |
    |           |_______map
    |           |         |
    |           |         |_______ckilogos.map
    |           |
    |           |
    |           |______tfm
    |           |        |
    |           |        |_______ckilogos.tfm
    |           |
    |           |
    |           |_______truetype
    |                          |
    |                          |_______ckilogos.ttf
    |
    |_______tex
              |
              |_______latex
                          |
                          |_______uscki.sty

Voer vervolgens MiKTeX Options (admin) als administrator uit.
Klik op het tablad  _roots_  en voeg de  _texmf_-map die je hebt aangemaakt toe.
Ga vervolgens naar het tabblad  _general_  en klik op  _Refresh FNDB_

Als het goed is, kun je nu de uscki-package in elk LaTeX-bestand op de computer gebruiken.

Als je geen MiKTeX geïnstalleerd hebt, weet ik het ook niet.
Ik heb dit zelf getest op Ubuntu en op Windows. Hoe het onder andere besturingssystemen werkt, weet ik niet.
