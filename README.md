# Respositori de notícies

**Aleix Martínez** i **Ignasi Vilarasau**

## Context

La realització d'aquesta pràctica s'ha dut a terme en el context de l'assignatura _Tipologia i cicle de vida de les dades_ del Màster de _Data Science_ de la _Universitat Oberta de Catalunya (UOC)_.
En concret en aquesta pràctica ens hem centrat en les dues primeres fases del cicle de les dades, la captura i l'emmagatzematge, utilitzant tècniques de _Web Scraping_. 

## Descripció

Imaginem, per exemple, que una marca de roba vol publicitar-se en la pàgina web d'un diari per intentar guanyar nous clients. En aquest sentit, al diari li interessaria poder disposar d'un dataset propi creat amb tot la informació relacionada amb l'històric de notícies que han anat publicat durant un període de temps en la seva pàgina web i en funció dels resultats de l'estudi de mineria de dades poder oferir una proposta de pressupost a la marca de roba interessada en publicitar-se.

D'aquesta forma hem decidit encarar la pràctica en aquest sentit. Hem recopilat informació relacionada amb les notícies publicades en la pàgina web del diari el País ([El País](http://www.elpais.com/)) per poder crear un dataframe com a respositori de dades on hi hagi suficient informació emmagatzemada, per a què, finalment puguem estudiar quines notícies acaben sent més vistes i perquè. I d'aquesta forma poder oferir-li aquest repositori i anàlisi al diari per a que pugui negociar amb propostes de pressupost més alt a marques que volen publicitar-se en la pàgina web del diari.

Per crear el dataset el que hem fet ha estat anar desant les dades necessàries extretes de la pàgina web del diari El País mitjançant un script (_WebScraping_ElPais_.ipynb_) que captura les dades i les guarda en un dataset descarregable localment. Finalment aquests datasets diaris (que contenen informació d'un dia en concret de la pàgina web d'El País) els hem unit per acabar creant el dataset definitiu on s'hi emmagatzema informació de diversos dies per poder realitzar els anàlisis pertinents per poder acabar obtenint informació valuosa que suposaria, pel diari, poder negociar contractes més bons amb les companyies publicitàries.

El dataset final hem decidit que hauria d'incloure com a mínim els següents atributs:
* **_Extraction Date_:** La data de la captura de les dades de la pàgina web del diari.
* **_Extraction Hour_:** L'hora de la captura de les dades de la pàgina web del diari.
* **_Publication Date_:** La data de publicació de l'article en el diari.
* **_Publication Hour_:** L'hora de publicació de l'article en el diari.
* **_Title_:** Títol de l'article publicat en el diari.
* **_Author_:** Autor de l'article del que hem emmagatzemat l'hora i dia de publicació, el títol.
* **_Location_:** Ubicació del succés que explica la notícia.
* **_Num Comments_:** Número de comentaris realitzats per usuaris registrats en la pàgina web del diari en la notícia.
* **_Photo Author_:** Autor o propietari de la fotografia que acompanya l'article.
* **_Photo Text_:** Text del peu de foto de la fotografia que acompanya l'article.
* **_Section_:** Secció a la que pertany la notícia emmagatzemada.
* **_Subsection_:** Subsecció a la que pertany la notícia emmagatzemada.


## Fitxer de codi utilitzat per realitzar _Web Scraping_:

* **WebScraping_ElPais.ipynb:** Script que permet extreure informació de la pàgina web.  Per fer això s'ha discretitzat el codi HTML de la pàgina web fins a les seves unitats mínimes que són els articles o les notícies. Definint un conjunt de funcions enfocades a extreure cadascún dels atributs anteriorment esmentats i posteriorment unir-los per escriure-ho en un fitxer. L'execució del codi procedeix a una descarrega automàtica del dataset creat amb un nom que inclou la data i hora d'extracció.
* **ElPais_Analysis.ipynb:** En aquest script proposem una possible via d'anàlisi per al dataset complert (que també creem en aquest script) que podria acabar amb unes conclusions interessants pel diari en qüestió. Aquest script també aporta una petita visualització del dataset.

## Bibliografia:

1. Lawson, R. (2015). **_Web Scraping with Python_**. Packt Publishing Ltd. Chapter 2. Scraping the Data.
2. Mitchel, R. (2015). **_Web Scraping with Python: Collecting Data from the Modern Web_**. O'Reilly Media, Inc. Chapter 1. Your First Web Scraper.
3. Simon Munzert, Christian Rubba, Peter Meißner, Dominic Nyhuis. (2015). **_Automated Data Collection with R: A Practical Guide to Web Scraping and Text Mining_**. John Wiley & Sons
4. Subirats, L., Calvo, M. (2018). **_Web Scraping_**. Editorial UOC.
5. Masip, D. (2010). **_El lenguaje Python_**. Editorial UOC.


